# Health survey from the CDC for relatable data science.

The data is a snapshot of the 2015-2019 Behavioral Risk Factor Surveillance System (BRFSS) survey from the US Center for Disease Control & Prevention (CDC). The source file can be accessed at: https://www.cdc.gov/brfss/

Variable types include: unordered categorical (nominal), ordered categorical (ordinal), binary, numeric.    
Only 2 missing points per observations were allowed (other instances were discarded).   
The full dataset (2015-2019) has over 2M rows. There are 295,550 observations in total in the most recent vintage (2019) when retaining instances with no missing point.

The shared files are:   
- the full dataset ([RData, 15Mo](/data/health_data.RData))  
- the cleaned 2019 vintage ([RData, 3Mo](/data/health_2019.RData))   
- the cleaned 2019 vintage ([zipped CSV, 4Mo](/data/health_2019.csv.zip))    

Examples of applications: [here](cdc_md.md).     
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
| **urban** | binary | whether respondent lives in metropolitan county (Yes or No)  | Low coverage in 2016 & 2017 |     
| **exercise** | binary | whether the respondent practiced exercise in the past month (Yes or No)  |  | 
| **smoker** | binary | whether the respondent has smoked 100 cigarettes in his life (Yes or No)  |     |  
| **fruit** | ordinal | frequency at which respondent eats fruits |  Not covered in 2016 & 2018 |  
| **coverage**|  binary | whether the respondent has any health care coverage (Yes or No) |  | 
| **health** | ordinal | feeling of respondent towards his/her health |    
