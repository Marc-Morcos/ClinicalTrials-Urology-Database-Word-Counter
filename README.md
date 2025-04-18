# Urology Database Word Counter
Script to analyze word usage in the U.S. National Library of Medicine ClinicalTrials.gov database. The keyword used was "Erectile Dysfunction". From this search, we downloaded the summary of the results in a csv file (ctg-studies.csv), then the details of each study as json files (ctg-studies.json.zip). 

Expected outputs are given in the "Output" folder for convenience. 
If you wish to filter for specific words, change the "wordsWeWant" variable in databaseWordCounter.py, then rerun(examples given in the comments on that line). 
If you wish to rerun the program, follow the instructions below.

To run:
- extract ctg-studies.json.zip into a folder called "ctg-studies"
- Delete the "Output" folder
- Install python 3.10.9 (https://www.python.org/). 
- Then, in the terminal, run
```
cd <path where you checked out this repository>
python -m pip install pandas==1.5.2 numpy==1.24.1 tqdm==4.64.1
python databaseWordCounter.py
```
The results will appear in a folder called "Output"

You can also get some extra data needed for the study into the console using
```
python otherDataFromStudies.py
```
and the outputs will appear under "Output/otherData" 
