# chaos-from-order
Replication materials for the paper, Chaos from Order: A Network Analysis of In-fighting Before and After El Chapo's Arrest

The subfolders and files contained in this folder can be used to reproduce the figures and statistical results from
the paper "Chaos from Order: The Effect of El Chapo's Arrest on In-fighting Networks." The files are structured as follows.

1. data: csv files used to create the network data
	1.1. ACLED.csv: Event data from Mexico that occcurred from 2018 to 2021
	1.2. input_data.csv: Event data from the other files in this folder that ocurred between 2012 and 2021, but not cleaned
	1.3. SCAD.csv: Event data from Mexico ranging from 1989 to 2021 that includes non-cartel and milita related events
	1.4. UCDP.csv: Event data from Mexico between 2012 and 2021

2. documents: Contains a codebook
	2.1. codebook.docx: The codebook

3. figures: all of the figures in the paper
	3.1. figure1.tiff
	3.2. figure2.tiff
	3.3 figure3.tiff
	3.4. figure4.tiff
	3.5. figure5.tiff
	3.6. figureA1.tiff

4. output: Contains the cleaned, merged, and deduplicated data used to produce the statistical results
	4.1. drugnet.csv: The cleaned, merged, and deduplicated data

5. scripts: A folder with the scripts used to generate the results in the paper
	5.1. step1.R: Cleans and deduplicates the input_data.csv data and writes the results to drugnet.csv in the output folder
	5.2. step2.R: Creates network objects, estimates SAOMs, and produces the figures from the article

6. Mexican Drug Cartel Rivalries.Rproj: An R Project file

7. readme.txt: The current file


The steps to reproduce the results are as follows:

	1. Double click on Mexican Drug Cartel Rivalries.Rproj. RStudio will open with both step1R and step2.R.
	
	2. Navigate to the step1.R script and use the cursor to highlight all of the code. Click "Run." Note that it is unecessary
		to set the working directory.

	3. Press Control + Shif + F10 or the equivalent keys on Apple or Linux systems.

	4. Navigate to the step2.R tab, highlight all of the code, and click "Run." It may take a long time to run this script
		because the blockmodels and SAOMs are computationally intensive. Note that running RSiena may also generate an
		output file.
