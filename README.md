# Health survey from the CDC for relatable data science.

The sample is a snapshot of the 2012-2020 Behavioral Risk Factor Surveillance System (BRFSS) survey from the US Center for Disease Control & Prevention (CDC). The source files can be accessed at: https://www.cdc.gov/brfss/

Variable types include: unordered categorical (nominal), ordered categorical (ordinal), binary and numeric - see table below.    
Only 2 missing points per observations were allowed (other instances were discarded).   
The full dataset (2012-2020) has over 3.7M rows.  
There are 295,550 observations in total in the most recent vintage (2019) when retaining instances with no missing point.

The shared files are:   
- the full dataset, 3.7M rows, 15 columns ([zipped RData, 26Mo](/data/health_data.RData)) (CSV file too large to be uploaded in GitHub - available upon request) 
- the cleaned 2019 vintage, 295K rows, 14 cols ([RData, 3Mo](/data/health_2019.RData)) ([zipped CSV, 4Mo](/data/health_2019.csv.zip))    

**DISCLAIMER**: the data is for pedagocial use only.  

More information & examples of applications via R code can be found [here](cdc_md.md).     
Variable description below.

|**Variable** | Type | Defintion |  Comments |
|---|---|---|---|
|**year** | numeric | year the survey was carried out (2015-2019)| |  
| **gender** | binary | respondent gender (Male or Female) |  |    
| **race** | nominal | respondent race  |   | 
| **age** | numeric | respondent age in years, capped above 80 |   | 
| **weight** | numeric | respondent weight in kilograms |  |
| **height**  |numeric | respondent height in centimeters  |  | 
| **education** | ordinal | maximum education level reached by the respondent  |  |
| **employment** | nominal | employment situation of the respondent |    |
| **income** | ordinal | annual income group of the respondent (household level) |   |
| **urban** | binary | whether respondent lives in metropolitan county (Yes or No)  | Low coverage before 2018 |     
| **exercise** | binary | whether the respondent practiced exercise in the past month (Yes or No)  |  | 
| **smoker** | binary | whether the respondent has smoked 100 cigarettes in his life (Yes or No)  |     |  
| **fruit** | ordinal | frequency at which respondent eats fruits |  Not covered in 2014, 2016 & 2018; low coverage in 2012 |  
| **coverage**|  binary | whether the respondent has any health care coverage (Yes or No) |  | 
| **health** | ordinal | feeling of respondent towards his/her health |    
