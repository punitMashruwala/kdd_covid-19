# Analysis of Measures taken by different countries to control the spread of Covid-19 Virus

This is a research project on the dataset which contains data of all the measures taken by different countries to control the **Covid-19 Pandemic**

Team Name: **Team RPM**

**Team Members:**

 - Nisha **R**amrakhyani - 801208678
 - Zalak **P**anchal - 801196881
 - Punit **M**ashruwala - 801208416

**Project Introduction:**
The project mainly focuses on the impact caused by different measures taken by different countries to control the spread of Covid-19. 
We have a dataset of around 22k records of measures taken by different countries along with the dates they started implementing these measures. 
We'll augment this dataset with the dataset of the number of Covid cases in each country each day. 
Our aim is to analyze the rise/fall in the number of Covid-19 cases before and after taking the necessary measures.

**Research Question:**

 - How did the different measures taken by different countries to
   control the Pandemic impact the total number of Covid-19 cases?

**Relevant Domain Information:** 

 - [https://www.acaps.org/covid-19-government-measures-dataset](https://www.acaps.org/covid-19-government-measures-dataset)
 - [https://en.wikipedia.org/wiki/Coronavirus_disease_2019](https://en.wikipedia.org/wiki/Coronavirus_disease_2019)

**Data Sources:**

 - [https://www.acaps.org/covid-19-government-measures-dataset](https://www.acaps.org/covid-19-government-measures-dataset)
 - [https://ourworldindata.org/covid-cases](https://ourworldindata.org/covid-cases)

**Approach:**

 - **Data understanding and EDA:**

	  

> **Introduction to the Dataset:**
> 
We are working on a dataset which contains record from the start of the first measure taken for the **Novel Coronavirus** which was later renamed to **Covid-19**.
> Our Dataset contains following columns: 
>  1   **ID** - Unique Number                  
 2   **ISO** - iso3 code                 
 3   **COUNTRY** - Name of the country                  
 4   **REGION** - Continent                  
 5   **LOG_TYPE** - Introduction / extension of measures, Phase-out of measures
 6   **CATEGORY** - Measures Category              
 7   **MEASURE** - Various method or rules applied to control the spread of the virus
 8   **TARGETED_POP_GROUP**   - Yes or no in dropdown     
 9   **COMMENTS**  - Comments or any others explanation for the measures      
 10   **NON_COMPLIANCE**  - Additional rules to applied like fines etc.
 11  **DATE_IMPLEMENTED** - Start of the measures in the country or part of the country       
 12  **SOURCE** - Data source for the mentioned Measures                 
 13  **SOURCE_TYPE** -  Data source type for the mentioned Measures         
 14  **LINK** - Link for the given information or data           
 15  **ENTRY_DATE** - Entry date of the given measure in the dataset          
 16  **covid_case_per_date** - Positive case found the given date of implementation of the measure.
 17  **population**  - Current population that country 
         
>  For more detail, please check this readme file:     
[https://www.acaps.org/sites/acaps/files/key-documents/files/acaps_-_covid-19_government_measures_dataset_readme.pdf](https://www.acaps.org/sites/acaps/files/key-documents/files/acaps_-_covid-19_government_measures_dataset_readme.pdf)

> 
> **EDA:**
> 
> We have used various visualization methods to analyze the correlation of each feature as part of EDA.
> More can be seen in the notebook in the folder with the name [**eda_code**](https://github.com/punitMashruwala/kdd_covid-19/tree/main/eda_code) or in the pdf file with the name: [**EDA - Jupyter Notebook.pdf**](https://github.com/punitMashruwala/kdd_covid-19/blob/main/EDA%20-%20Jupyter%20Notebook.pdf)


 - **Date Preparation:**
 
> - From 17 columns available in the dataset, we decided to drop some
   column and we selected the following columns:
     **COUNTRY**, 
 **CATEGORY**, 
 **MEASURE**, 
 **COMMENTS**,
**DATE_IMPLEMENTED**, 
**covid_case_per_date**, 
**population** 
And stored in this dataset in the variable **df**
> - We scaled the **covid_case_per_date** column data to normalize and stored in the column: **log_value**
> - Converted Datatype of Date column to DATETIME from OBJECT
> - Checked for null values in all the data frames. We found around 60 Null values in the dataset. So we decided to drop those null values rows. 
> - Now dataset was ready for modeling
 
   

 




 - **Machine Learning (if applicable - supervised, unsupervised):**
	  *This is a work in progress*
	  
 - **Evaluation:**
	  *This is a work in progress*

	  

**Known Issues (problems with predictors, reporting, bias, etc.)** 
			*This is work-in-progress*

**Conclusion**
			*This is work-in-progress*
