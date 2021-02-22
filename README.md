# DataManagement-and-Int
This is the first in a data science specialization, Data Analysis and Interpretation from Wesleyan University entitled Data Management and Visualization. I must pick a data set that I wish to study; this data set will be used for the entirety of the specialization. 
The course offers five distinct data sets or I may choose my own. I have decided to use one of the existing choices. It is a data set specific to a study of the craters of Mars in 2011, by Stuart James Robbins of the University of Colorado, Boulder. Links to the study, codebook and data set are in the References section at the bottom of this post.
I am interested in the physical characteristics of Martian craters, specifically diameter (DIAM_CIRCLE_IMAGE) and depth (DEPTH_RIMFLOOR_TOPOG). The morphology category data (MORPHOLOGY_EJECTA_1 through 3) is an interesting feature, however the data is overwhelmingly incomplete and not robust enough for sustained analysis and difficult to interpret based on my lay background in the field. The features are small enough to be inclusive, however I will be limiting my analysis to the following data fields:
1.	CRATER_ID: Crater ID for internal use, based upon the region of the planet (1/16ths), the “pass” under which the crater was identified, and the order in which it was identified.
2.	LATITUDE_CIRCLE_IMAGE: Latitude from the derived center of a non-linear least-squares circle fit to the vertices selected to manually identify the crater rim (units are decimal degrees North).
3.	LONGITUDE_CIRCLE_IMAGE: Longitude from the derived center of a non-linear least-squares circle fit to the vertices selected to manually identify the crater rim (units are decimal degrees East).
4.	DIAM_CIRCLE_IMAGE: Diameter from a non-linear least-squares circle fit to the vertices selected to manually identify the crater rim (units are km).
5.	DEPTH_RIMFLOOR_TOPOG: Average elevation of each of the manually determined N points along (or inside) the crater rim (units are km).
a. Depth Rim: Points are selected as relative topographic highs under the assumption they are the least eroded so most original points along the rim.
b. Depth Floor: Points were chosen as the lowest elevation that did not include visible embedded craters.
The raw data file may be viewed here: https://raw.githubusercontent.com/PittBuzz/DataManagement-and-Int/main/marscrater_data.csv
My initial analysis will be to determine if there is an association between crater diameter and depth in kilometers. Further I will conduct analysis to determine if there is a secondary association between the noted characteristics and crater location, time permitting. An additional consideration will have to be given to adapting any geo-spatial programs for Mars-specific coordinates.
Google Scholar has identified previous research on the characteristics of Mars craters obtained from the Mars Orbital Laser Altimeter. The study is listed below in the References section.
Crater studies date to the 1990s and earlier however the datasets are not relevant for the scope of this course. 
An initial null hypothesis is that crater diameter and depth do not have a direct correlation to each other. While H1 does posit a direct correlation. 
References
Robbins, S. J. (2011), Planetary Surface Properties, Cratering Physics, and the Volcanic History of Mars from a New Global Martian Crater Database., Site: Stuart Robbins, Astro/Geophysicist on the Web, 1–239, address: http://about.sjrdesign.net/files/thesis/RobbinsThesis_LargeMB.pdf, 
codebook: https://github.com/PittBuzz/DataManagement-and-Int/blob/main/Custom%20Mars%20Codebook.docx
Aharonson, O., M. T. Zuber, and D. H. Rothman (2001), Statistics of Mars’ topography from the Mars Orbiter Laser Altimeter: Slopes, correlations, and physical Models, J. Geophys. Res., 106(E10), 23723–23735, doi:10.1029/2000JE001403.
Data set: https://github.com/PittBuzz/DataManagement-and-Int/blob/main/marscrater_data.csv
