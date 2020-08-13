# cse6242_final_project

# Visualizing the relationship between School Quality and Real Estate Value in NYC

--------------------
*CONTENTS OF THE FILE
--------------------
* DESCRIPTION
* INSTALLATION
* EXECUTION

-----------
*DESCRIPTION
-----------
There are two main folders:

1) Machine Learning /CODE/MACHINE LEARNING/

	Machine Learning breaks out into two main processes:

		a) Real Estate Forecasting (There is one file)

			* Real_Estate_Forecasting.ipynb - Main file to be run in jupyter notebook

		b) School Quality Rating (There are three files)

			* ClassifySchoolQuality.py - Main execution file to be ran in command prompt and generate High School quality file
 			* preprocess.py - Clean and transforms values in dataset into more usable form
 			* ML.py - Train and build a prediction model using Random Forest

 		c) /data
 			This directory contains the input and output of our analysis (in a zipped file)
 			* 2020highschool.csv - input data for ClassifySchoolQuality.py
 			* SchoolQualityResponse.csv - input data for ClassifySchoolQuality.py
 			* school_quality_rating.csv - output of running ClassifySchoolQuality.py
 			* homedata.csv - input data of average home prices in american towns from 1996-2020
 			* pricedata.csv - output of running Real_Estate_Forecasting.ipynb

2) Visualization /CODE/Visualization

	The data visualization is an HTML file which uses D3 and Leaflet.

	* NeighborhoodMap.html - Main file with visualization code
	* /lib - directory of various libraries used in NeighborhoodMap.html
	* /Project6242 - other supporting files
	* /data - data used in the visualization
		* borders.json - All of our custom region borders from combining school districts with neighborhoods
		* pricedata.csv - Cleaned real estate valuation
		* school_quality_rating.csv - School rating data


------------
*INSTALLATION
------------

1) Machine Learning

	Download Anaconda (Python Version 3.7)



---------
*EXECUTION
---------


1) Machine Learning (first unzip data in ~/CODE/MACHINE LEARNING/DATA)

	a) Real Estate Forecasting (Estimated Execution time ~3 mins)

		1. Download Machine Learning Folder
		2. Open up jupyter notebook (from anaconda download)
		3. Navigate to and run Real_Estate_Forecasting.ipynb
		4. A CSV name "pricedata.csv" will be saved to your machine which will be utilized for the visualization step

	b)  School Quality Rating (Estimated Execution time ~1 min)
		1. Open command prompt and run a following code: python ClassifySchoolQuality.py
		2. school_quality_rating.csv file will be saved in current folder where the code is located
		3. This CSV file will be used for visualization part in the project


2) Visualization

	1. Navigate to /CODE/Visualization in your terminal
	2. Run the command "python -m http.server" to start a server
	3. Open firefox in private browsing mode and go to http://localhost:8000/ and open NeighborhoodMap.html


-----------------------------------------------------------------------------
