# US Residential Energy Adoptions

## Dataset Description  
This dataset, published in *Scientific Data* (Fuentes et al. 2025), provides self-reported information on residential energy decisions across the United States. Covering the period 2010–2023, the survey-based data captures household adoption patterns for rooftop solar, electric vehicles, and heat pumps, alongside demographic and socioeconomic attributes. Respondents provided insights into motivations, barriers, and perceptions influencing their technology choices.  

The dataset is valuable for analyzing equity and accessibility in the U.S. energy transition, as it links adoption outcomes to household characteristics such as income, education, and geography. It offers opportunities to apply machine learning methods to predict adoption likelihood, identify systemic disparities, and inform policy design.  

---

## Data Dictionary  

## Data Dictionary  

| Column Name                        | Description                                                                                                   | Type        |
|------------------------------------|---------------------------------------------------------------------------------------------------------------|-------------|
| `geo_state_zip`                    | QA/QC of respondent reported state & ZIPCODE                                                                  | String      |
| `geo_review`                       | Paste of `state_chk`, `zcta_chk`, `county_chk`                                                                | String      |
| `state_chk`                        | Whether reported state is same as IP address state                                                            | Binary      |
| `zcta_chk`                         | Whether reported state is same as assigned ZCTA                                                               | Binary      |
| `county_chk`                       | Whether assigned county (from ZCTA) is same as IP address county                                               | Binary      |
| `region`                           | Region of US assigned, based on assigned state                                                                | Categorical |
| `assigned_state`                   | State assigned by researchers (uses reported state unless missing, then IP address state)                      | Categorical |
| `reported_state`                   | State respondent claimed as residence                                                                         | Categorical |
| `zcta_state`                       | State in which assigned ZCTA occurs                                                                           | Categorical |
| `assigned_county_fip`              | 5-digit ID code for assigned county                                                                           | Integer     |
| `assigned_county`                  | Name of county assigned based on ZCTA                                                                         | Categorical |
| `urb_rural`                        | Urban or Rural classification                                                                                 | Categorical |
| `IECC15`                           | Climate Zone (International Energy Conservation Code 2015), values 1–7                                        | Integer     |
| `IECC21`                           | Climate Zone (International Energy Conservation Code 2021), values 1–7                                        | Integer     |
| `BA15`                             | Building America Climate Zone (IECC 2015): Hot-Humid; Mixed-Humid; Hot-Dry; Mixed-Dry; Cold; Very-Cold; etc.   | Categorical |
| `BA21`                             | Building America Climate Zone (IECC 2021): Hot-Humid; Mixed-Humid; Hot-Dry; Mixed-Dry; Cold; Very-Cold; etc.   | Categorical |
| `Moisture15`                       | Moisture Code (IECC 2015): A, B, or C                                                                         | Categorical |
| `Moisture21`                       | Moisture Code (IECC 2021): A, B, or C                                                                         | Categorical |
| `USDA_Hardiness_Zone`              | USDA plant hardiness zone (based on ZCTA)                                                                     | Integer     |
| `USDA_temp_range`                  | USDA plant hardiness temperature range (based on ZCTA)                                                        | String      |
| `USDA_Zone_Title`                  | USDA plant hardiness zone title (based on ZCTA)                                                               | String      |
| `own_rent`                         | Own or rent current home                                                                                      | Categorical |
| `reported_age`                     | Respondent age                                                                                                | Integer     |
| `children`                         | Number of children in household (≤17)                                                                         | Integer     |
| `age18_64`                         | Household composition: Adults aged 18–64                                                                      | Integer     |
| `age65plus`                        | Household composition: Older adults aged 65+                                                                  | Integer     |
| `hh_size2`                         | Total household size (all age groups, including respondent)                                                    | Integer     |
| `userlanguage`                     | Language in which survey was conducted                                                                         | Categorical |
| `hometype`                         | Type of home: Single-family, condo/apartment (≤4 units), duplex/triplex/townhouse                              | Categorical |
| `gender`                           | Gender identity                                                                                               | Categorical |
| `race_americanindianoralaskannati` | 1 if respondent identified as American Indian or Alaska Native, 0 otherwise                                   | Binary      |
| `race_asian`                       | 1 if respondent identified as Asian, 0 otherwise                                                              | Binary      |
| `race_blackorafricanamerican`      | 1 if respondent identified as Black or African American, 0 otherwise                                          | Binary      |
| `race_middleeasternornorthafrican` | 1 if respondent identified as Middle Eastern or North African, 0 otherwise                                    | Binary      |
| `race_nativehawaiianorotherpacifi` | 1 if respondent identified as Native Hawaiian or Other Pacific Islander, 0 otherwise                          | Binary      |
| `race_otherpleasespecify`          | 1 if respondent identified as Other, 0 otherwise                                                              | Binary      |
| `race_prefernottosay`              | 1 if respondent preferred not to say, 0 otherwise                                                             | Binary      |
| `race_white`                       | 1 if respondent identified as White, 0 otherwise                                                              | Binary      |
| `ethnicity_all`                    | Hispanic/Latino heritage (yes/no)                                                                              | Binary      |
| `education`                        | Highest level of education obtained                                                                            | Categorical |
| `hhincome`                         | Household annual income                                                                                       | Continuous  |
| `mortgagerent`                     | Monthly housing cost (mortgage or rent, narrow range)                                                         | Continuous  |
| `mortgagerentbins`                 | Monthly housing cost (broader range)                                                                          | Categorical |
| `homeyrs`                          | Number of years living in current home                                                                        | Integer     |
| `yrbuilt`                          | Year home was built                                                                                           | Integer     |
| `homesqft`                         | Home size in square feet                                                                                      | Continuous  |
| `heatsource`                       | Main fuel used to heat home                                                                                   | Categorical |
| `waterheatsource`                  | Main fuel used for water heating                                                                              | Categorical |
| `energyexpenses`                   | Average monthly energy expenses                                                                               | Continuous  |
| `electricgasbill`                  | Trouble paying electric/gas bill each month (yes/no)                                                          | Binary      |


---

## Reflection on Replicability and Reuse  

This dataset is **FAIR-compliant**: it is openly available, well-documented, and structured for interoperability across statistical and ML tools. Its survey-based nature introduces self-reporting bias and geographic sampling limitations, but transparent methodology enhances replicability.  

For **reuse**, the dataset is highly versatile: social scientists can study behavioral and equity dimensions of energy adoption, while machine learning researchers can benchmark predictive models for technology diffusion. Because the dataset is anonymized and aggregated responsibly, it adheres to ethical reuse guidelines while aligning with **CARE principles**, particularly in ensuring benefits for underserved communities in energy transitions.  
