[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fangyf113/testvoilawork699/main?urlpath=voila%2Frender%2FOutput%20(1).ipynb)


<h1 align="center">CFPB Complaints Analysis </h1>
<h3 align="left">This project is the final result for course Capstone SIADS 699.</h3>

<h4 align="left">Data Source:https://www.consumerfinance.gov/data-research/consumer-complaints/</h4>
<p align="left">
</p>
<h5 align="left">The datasource is owned by CFPB, and it could be access through downloading in a csv file or using API. For this project, I have downloded the dataset into a csv file. But this file is greater than 1GB, thus not included in this repository. But a smaller csv could be downloaded through the link above. </h5>
<p align="left">
</p>

<h4 align="left">Languages and Tools:</h4>
<p align="left"> <a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> </p>


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Setup](#setup)
* [Usage](#usage)
* [Project Status](#project-status)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)
<!-- * [License](#license) -->


## General Information
- The project focuses on CFPB complaint and the data is made publicly available through the CFPB website. The CFPB collects the complaints, then sends them to the financial services companies for a response. We are interested in analyzing the complaints over time, company responses, and ongoing trends in the complaint data.

- For this project, we focused on topic extraction from complaints narratives.
- With the topic modelling, and the final output interface, the intention is to help CFPB to accelerate the complaint process, and be able to track topic models trend and patterns in complaint narrative. And with the interface, it is easy to predict the main topic on any new complaint narrative.


## Technologies/Environment Used
- AWS SageMaker
- Great Lake


## Setup
A requirements.txt in the folder which specified all the requirement packages needed for the project.
Another requirement.yml file which is needed for the setup for Binder to display the interface. It is not required if you need to run the project on your own laptop. 


## Structure
Three main jupyter notebooks are the output for this project. 
1. EDA - this jupyter notebook has Exploratary Data Analysis and focuses on visualzing some metrics such as complaints timely responce, and time gaps between a complaints gets received and complaint sent to companies.
2. Data Cleaning & Topic Modeling - this is the main notebook that has the data cleaning stepa, and the topic modeling part.
3. Output-interface - this is where we apply the model and accepts new complaint narrative and predict the major topic model.
4. requirement.txt - This is file lists all the packages and libraries that we may need for the project.
5. All other files - all the models and id2words and bigrams are saved so that if you would not like to re-run the project from the scratch, these results could be simply load to show the results.



## Project Status
Project is: _complete_ 

## Room for Improvement
Include areas you believe need improvement / could be improved. Also add TODOs for future development.

Room for improvement:
- The current topic modeling is based on coherence value, future improvement could be using clustering as method to pick the most appropriate number of topics for the topic modeling.
- The current final interface only takes the complaint narrative and predict the main topic. Due to the limitation of the server, more visualizations could not been shown, so in the future, we could consider to switch to another platform.
