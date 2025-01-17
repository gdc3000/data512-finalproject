Examining the link between temperature and violent crime in Seattle
Author: Geoff Coyner

Abstract
This project examines the link between violent crime and temperature in Seattle. Several studies of Chicago and one of Finland suggest a positive relationship between temperature and violent crime. Since climate studies indicate Seattle will see a 3-10 degree F temperature increase over the next century, a link here would suggest a need to plan for climate related crime in Seattle. After looking at data between 2012 and 2017, I am unable to find a clear link between temperature and crime in Seattle. Instead, I find a much stronger link between crime and month of the year, time of day and day of the week, when controlling for temperature. While more research should be done to expand upon this work, initial findings suggest the link between violent crime and temperature should not be a factor in law enforcement decision-making in Seattle.

Overview
This readme walks through the files that can be found in the github repo, how they are relevant to my project and how my project can be reproduced using the data and Jupyter notebook contained in the repo.

My final write-up and full analysis is documented in the file "hcds-a6-finalproject.ipynb".

All data used is publicly available. A key goal of this project is to practice and show-case open scientific research best practices so that this study can easily be replicated or expanded upon.

This work is shared under and MIT license.

Getting Started
These instructions will get you up and running and explain the project, data and relevant files in more detail. The source data is included in the repo and the final written report, data gathering processing and analysis steps to recreate the study in its entirety can be found in the Jupyter notebook in the repo (each file in the repo is described in more detail below). The entire workflow from data acquisition, processing and acquisition can be reproduced through the included Jupyter notebook.

Before attempting to reproduce this work, please ensure that Jupyter notebooks is installed on local machine or accessible online and Python v3.6 is installed where appropriate.

Contents of this repo
This repo contains the following files:
	� 1 Jupyter notebook file called "hcds-a6-finalproject.ipynb" including a written report describing my study and outlining in detail the steps of data acquisition, processing and analysis. Included in the analysis steps (Step 3) are heatmaps and regression analysis results referred to throughout the written report, especially in the section called Findings.
	� 2 .csv files called "Seattle_Police_Department_Police_Report_Incident.csv" and  "Seattle_Police_Department_Police_Report_Offense.csv", which was the source of the crime data in the analysis. The incident file is a compressed version of the file downloaded from Seattle PD. Several irrelevant fields were manually removed from the GIT version in order to reduce the file size.
	� 1 .csv files called "sunrise_sunset.csv" which was the source of the sunset and sunrise times used in determining whether a given hour was light or dark in the analysis.
	� 1 text document called "asos.txt" which was the source of the weather data used in the analysis.
	� 1 Readme file
	� 1 License file

Relevant Documentation and Source Data
This project is based entirely on publicly available data.

Asos.txt is made available by Iowa State University under an MIT license. The original source of the data is the airport AWOS (Automated Weather Observation Systems) at various airports around the nation, which are published by NOAA and considered public information. Data was pulled from January 2012 through November 2017.

The crime incident and offense data is made available under a Creative Commons license by the city of Seattle. This data was pulled from January 2012 through November 2017.

The sunrise and sunset data are made available by the US Naval Observatory. Because the US Naval Observatory is a US Federal Government agency, this data is considered public information.

Web links to source data and other resources are available in the Jupyter notebook.

Limitations of the data
The AWOS data does have occassional gaps due to malfunctioning sensors or missing records. These are analyzed in the data processing steps in the Jupyter notebook, removed before analysis is performed and deemed not to cause significant impact to the study. 

The police data is based on incidents reported, is unfiltered and does not include information about whether or not the criminal incident actually occurred as described or if anyone was later found guilty. In conducting this study, we assume incidents which do not result in a conviction or which were misreported occur at random and therefore should not be related to a correlation between temperature and crime or impact a study of this relationship.

Licenses
This project is licensed under the MIT License. See the�license file for more details. 

The Seattle PD makes their data available under a Creative Commons Attribute-ShareAlike License.

Iowa State University makes their data available under an MIT license.

All US Naval Observatory data is considered public information.

Python and python standard library packages are available under a modified GPL-compatible license. The pandas package is available under the 3-clause BSD license. NumPy, Math, Seaborns and StatsModel are licensed under the�BSD license. Datetime is licensed under a Zope Public License.