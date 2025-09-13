# Dataset Documentation  

## Dataset Description  
This dataset, published in *Scientific Data* (Fuentes et al. 2025), provides self-reported information on residential energy decisions across the United States. Covering the period 2010–2023, the survey-based data captures household adoption patterns for rooftop solar, electric vehicles, and heat pumps, alongside demographic and socioeconomic attributes. Respondents provided insights into motivations, barriers, and perceptions influencing their technology choices.  

The dataset is valuable for analyzing equity and accessibility in the U.S. energy transition, as it links adoption outcomes to household characteristics such as income, education, and geography. It offers opportunities to apply machine learning methods to predict adoption likelihood, identify systemic disparities, and inform policy design.  

---

## Data Dictionary  

| Column Name             | Description                                                      | Type        |
|--------------------------|------------------------------------------------------------------|-------------|
| `respondent_id`          | Unique anonymized identifier for each household                 | Integer     |
| `year`                   | Survey year (2010–2023)                                         | Integer     |
| `state`                  | U.S. state of residence                                         | Categorical |
| `income_bracket`         | Reported household income range                                 | Categorical |
| `education_level`        | Highest level of education attained                             | Categorical |
| `housing_type`           | Type of residence (single-family, multi-family, rental, etc.)   | Categorical |
| `solar_adoption`         | Indicator of rooftop solar adoption (1 = yes, 0 = no)           | Binary      |
| `ev_adoption`            | Indicator of electric vehicle ownership (1 = yes, 0 = no)       | Binary      |
| `heat_pump_adoption`     | Indicator of heat pump adoption (1 = yes, 0 = no)               | Binary      |
| `decision_factors`       | Self-reported drivers (e.g., cost, environment, reliability)    | Text        |
| `barriers`               | Reported barriers to adoption (e.g., upfront cost, awareness)   | Text        |
| `policy_awareness`       | Awareness of incentives or state/federal policies (1/0)         | Binary      |

*(Table simplified for subset; see original publication for full schema.)*  

---

## Reflection on Replicability and Reuse  

This dataset is **FAIR-compliant**: it is openly available, well-documented, and structured for interoperability across statistical and ML tools. Its survey-based nature introduces self-reporting bias and geographic sampling limitations, but transparent methodology enhances replicability.  

For **reuse**, the dataset is highly versatile: social scientists can study behavioral and equity dimensions of energy adoption, while machine learning researchers can benchmark predictive models for technology diffusion. Because the dataset is anonymized and aggregated responsibly, it adheres to ethical reuse guidelines while aligning with **CARE principles**, particularly in ensuring benefits for underserved communities in energy transitions.  
