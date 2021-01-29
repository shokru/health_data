# Dataset from the CDC for relatable data science.

The data is a snapshot of the 2019 Behavioral Risk Factor Surveillance System survey from the US Center for Disease Control & Prevention (CDC). The source file can be accessed at: https://www.cdc.gov/brfss/annual_data/annual_2019.html

Variable type includes: unordered categorical (nominal), ordered categorical (ordinal), binary, numeric.   
There are 295,550 observations in total in the most recent vintage (2019).

|**Variable** | Type | Defintion |  Comments |
|---|---|---|---|
|**year** | numerical | year the survey was carried out (2015-2019)| |  
| **gender** | binary | respondent gender (Male or Female) |  |    
| **race** | nominal | respondent race  |   | 
| **age** | numeric | respondent age in years, capped above 80 |   | 
| **weight** | numeric | respondent weight in kilograms |  |
| **height**  |numeric | respondent height in centimeters  |  | 
| **education** | ordinal | maximum education level reached by the respondent  |  |
| **employment** | nominal | employment situation of the respondent |    |
| **income** | ordinal | annual income group of the respondent (household level) |   |
| **urban** | binary | whether respondent lives in metropolitan county (Yes or No)  | Low coverage 2016 & 2017 |     
| **exercise** | binary | whether the respondent practiced exercise in the past month (Yes or No)  |  | 
| **smoker** | binary | whether the respondent has smoked 100 cigarettes in his life (Yes or No)  |     |  
| **fruit** | ordinal | frequency at which respondent eats fruits |  Not covered in 2016 & 2018 |  
| **coverage**|  binary | whether the respondent has any health care coverage (Yes or No) |  | 
| **health** | ordinal | feeling of respondent towards his/her health |    
