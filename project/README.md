# Title
Are we eating the foods when we are supposed to?
 
# Abstract
#### A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?
 
The aim of this project is to figure out if the foods that grow during precise natural seasons are actually eaten during that time. Based on the access pattern of recipes in the recipes dataset, we can build consumption patterns for given foods in relation to location and time of the year. That combined with data about those foods and particularly what season they grow and natural area of production from an encyclopedia dataset, will allow us to draw conclusions if the foods were imported from far away. There are two possible reasons for a food to be imported: it is not native to that region or it is not a season for that food production. As a result, there are two side effects of imported foods: there is a greater harm to the environment and a harm to the local economy by overstepping local producers. This study is designed to promote local ecological food production by building a case for conscious food consumption.
 
 
# Research questions
#### A list of research questions you would like to address during the project. 
 
- Do people choose recipes that use foods from the current season and locally grown?
- Are recipes chosen by users based on the season?
- Do recipe websites propose recipes in line with the current season?
 
# Dataset
#### List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.
 
- The main dataset will be Stanford infolab’s cooking recipe dataset
- We will also explore if there are datasets that can tell us about food shopping patterns in US food retail stores
- Moreover we will need data about the foods, time of the year when it is grown and native location. This can be found in Wikipedia, we will consider other datasets as well.
 
 
# A list of internal milestones up until project milestone 2
- Start collecting and parsing the data to verify that it is usable in its entirety
- Setup the data analysis bases in a notebook
- Search for other databases in link with food purchase/consumption by time of the year
- See how we can extract food season from e.g. Wikipedia page or other source
- Look up scientific papers or simply articles about seasonal food and its public perception/knowledge in the USA
 
 
 
# Questions for TA
- Do you think we have a substantial enough idea for completing a good project, or should we explore more questions, or another angle of the seasonal food question?
- Do you have any tips on how to find the food season for a particular food?

# Source
#### GeoJson: 
http://eric.clst.org/Stuff/USGeoJSON


# Milestone 2
- We have created the base of our Pipeline and are loading data from multiple websites from the dataset. We came across many issues during the development of our project:
  * Most of the data from the different websites doesn't contain a usable date. We needed to be able to tell when the recipe was consumed by the user, so we finally settled on taking the date of the recipe review (rating), which is an information that some websites contain.
  * The dataset doesn't contain raw data, but are html dumps of the websites. We need to do a lot of pre-processing to extract the useful information, which takes a lot more time than anticipated. (different encodings, missing data, non-consistent data, ...).
  * As the dataset is formed from many different websites, there is sometime s great disparity in the collected the data, therefore we have to get a lot of data so that it's concluant enough.
- We have found a few websites that contain the food's season, to be able to show if it's correlated with the food season
- We still have to complete the process and get conclusions. Then, depending on the latter, we will see if we can find reasons to explain them in papers or articles.
