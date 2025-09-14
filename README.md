# Residential Energy Adoption in the U.S.  
**Shehr Naz Ashraf – PS1**  

## Abstract  
This project investigates the social and technological determinants of residential adoption of energy-efficient and renewable technologies in the United States. Using the open-access dataset from *Nature Scientific Data* (Fuentes et al. 2025), which documents household-level adoption of rooftop solar, electric vehicles (EVs), and heat pumps, the research proposes a machine learning–augmented analysis to examine how socioeconomic, demographic, and geographic factors shape technology diffusion.  

The study frames its inquiry at the intersection of social science and machine learning, guided by the AI Triad: **data** (large-scale household adoption dataset), **algorithms** (ML models for prediction and feature attribution), and **computing power** (scalable training environments). By combining traditional literature review and GenAI-assisted workflows, this project aims to generate insights relevant to equity in the U.S. energy transition and advance reproducible practices under the FAIR and CARE principles.  

---

## System Configuration  

### Local Setup  
- **Python Version**: 3.10+  
- **Dependencies**:  
  ```bash
  pip install -r requirements.txt

where requirements.txt includes:
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
- jupyter
- Execution: Open code/eda.ipynb in Jupyter Lab/Notebook to reproduce exploratory analysis.


## Cloud Setup

### Google Colab
Clone repo and run:
```
!git clone https://github.com/Rising-Stars-by-Sunshine/<your-repo-name>.git
%cd <your-repo-name>/code
```

### AWS EC2:
- Launch Ubuntu instance (t2.medium or above recommended).
- Install Anaconda or Miniconda.
- Run Jupyter Notebook server for interactive analysis.


## FAIR & CARE Principles

FAIR: Dataset is findable (hosted on Nature Scientific Data & Kaggle), accessible (open license), interoperable (structured tabular format), and reusable (documented variables).

CARE: While U.S.-focused, analysis is conducted with attention to equity and responsibility in how ML insights may affect underrepresented communities. Transparency in modeling and acknowledgment of potential biases will be prioritized.


## Repository Structure
```
├── README.md                <- Project overview (this file)
├── data/
│   ├── UPGRADE-E_V2.csv     <- Open-source dataset subset
│   └── README.md            <- Dataset description + dictionary
├── code/
│   ├── eda.ipynb           <- Exploratory Data Analysis notebook
└── README.md               <- Summary of analysis code
```

## References
Fuentes, T. L., K. H. McCord, M. J. Martell, et al. 2025. “A Dataset for Understanding Self-Reported Patterns Influencing Residential Energy Decisions.” Scientific Data 12: 1273. https://doi.org/10.1038/s41597-025-05335-8
