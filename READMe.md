{\rtf1\ansi\ansicpg1252\cocoartf2822
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fnil\fcharset0 .AppleSystemUIFontMonospaced-Regular;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;}
\paperw11900\paperh16840\margl1440\margr1440\vieww12120\viewh12240\viewkind0
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0

\f0\fs26 \cf2 # Car Price Prediction\
The core of this project is exploring the key factors that influence car prices for used cars, using regression models and feature engineering.\
\
## Overview\
We follow the CRISP-DM method to examine what features of a used car drive its price. The data is from a Kaggle set of used cars that contains $426,000 cars. It was scrapped off a national USA, used car website and placed onto the Kaggle website. It was provided to us as a .csv by our course administration.\
\
## Contents\
In this repository is the Jupyter Workbook that was used to do feature engineering on the data set. There is the data directory/folder containing one .csv file with the date. There is also a directory/folder called \'93data\'94for two .jpg image files that came with the original get displayed in the Jupyter Workbook. The Jupyter Workbook creates a directory for results images called images_of_results. Two .jpg image files are created and stored in that directory by the workbook and those images are displayed in the \'91Deployment\'92 section at the bottom of the workbook in the final business report:\
     relative_importance_top7.jpg - bar chart of the feature importance\
     top_features_table.jpg - table of the most important values\
\
## How to Run\
Load the Jupyter into a suitable platform (Colab/Anaconda etc) and ensure the platform has access to the data and images.\
\
## Results\
We found that a model can be build that relies heavily on these main features: year, cylinders, odometer and manufacturer. The year is by far the most influential on the price then cylinders and odometer are similar. Next is the manufacturer and then a big drop to state.\
\
Ridge regression was found to provide the best refinement of a polynomial model of degree 5. This 5 degree polynomial allows for non-linear, complex patterns in the data to be modelled. A plot was made of the model\'92s curve for year against price. This reveals the year\'92s complex curative that required a degree 5 polynomial to model its very high influence on the model.\
\
We also determined which particular entries of those influential features are valued the most. Starting with the most influential and then listing the next three with decreasing influence, they are:\
\
1. **year**\
   The most valued 10 year period is 2020-2029, followed by 1910-1919, then 1930-1939.\
   \
2. **cylinders**\
   The most valued are 12 cylinder vehicles, followed by 8 cylinder vehicles.\
\
3. **odometer**\
   The most valued are cars with under 24,471 km on the odometer (top decile = top 10%).\
\
4. **manufacturer**\
    The most valued manufacturers are: Ferrari, Aston-Marton and Tesla.\
}