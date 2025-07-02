# CVE Risk Assessment Using EPSS: Machine Learning Approach

## 📋 Project Overview

This repository contains the code and data for our thesis on **"Automated Vulnerability Risk Assessment Using Machine Learning and EPSS (Exploit Prediction Scoring System)"**.

## 🎯 Research Objective

Our research focuses on developing machine learning models to predict EPSS scores for Common Vulnerabilities and Exposures (CVEs) using their metadata and characteristics. This enables automated risk assessment and prioritization of vulnerabilities for security teams.

## 📊 Dataset

- **602 CVE records** from 2023-2025
- **EPSS scores** (Exploit Prediction Scoring System)
- **CVSS v3.1 scores** (Common Vulnerability Scoring System)
- **Vendor and product information**
- **Exploitation status data**

## 🗂️ Repository Structure

```
├── code/
│   ├── 31xxx/                    # CVE JSON files (160+ records)
│   ├── Mubaraq.ipynb            # Main analysis and ML modeling
│   ├── Init.ipynb               # Environment setup
│   ├── cve_data_with_epss.csv   # Main dataset
│   ├── extreme_cases_analysis.csv # Prediction analysis
│   ├── requirements.txt         # Python dependencies
│   └── *.parquet               # Efficient data storage
├── README.md                    # This file
├── LICENSE                      # MIT License
└── .gitignore                  # Git ignore rules
```

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Required packages (see requirements.txt)

### Installation
```bash
# Clone the repository
git clone https://github.com/mubaraqx/EPSS_challenge25.git
cd EPSS_challenge25

# Install dependencies
pip install -r code/requirements.txt

# Start Jupyter
jupyter notebook
```

### Usage
1. Open `code/Init.ipynb` to set up the environment
2. Execute `code/Mubaraq.ipynb` for the main analysis

## 📈 Key Findings

- **Machine learning models** can effectively predict EPSS scores
- **CVSS scores, vendor information, and CWE codes** are important features
- **XGBoost** performs well for this regression task
- **Feature engineering** from CVE descriptions improves accuracy

## 🔬 Methodology

1. **Data Collection**: CVE data from NVD and EPSS scores
2. **Feature Engineering**: Text processing, categorical encoding
3. **Model Development**: XGBoost, Random Forest, Neural Networks
4. **Evaluation**: MSE, MAE, and extreme cases analysis
5. **Validation**: Cross-validation and holdout testing

## 📚 Thesis Reference

This code accompanies our thesis: **[Open-Source Vulnerability Risk Assessment: A Machine Learning Approach Using Public Data]** by [Mubaraq M. Fuseini], [Almustafa Almuthana], [Abdullah Abdelkhalik]

**Abstract**: [The Exploit Prediction Scoring System (EPSS) has become the indus-
try standard for vulnerability risk assessment, yet its proprietary
nature creates significant barriers to transparency and independent
validation. This thesis challenges the assumption that effective vul-
nerability exploitation prediction requires proprietary datasets by
developing a fully transparent system using only publicly available
data sources.
We built a vulnerability exploitation prediction system that lever-
ages ExploitDB[1] as its primary dataset, supplemented by NVD[2]
and CISA[3] data. Our approach combines manual data collection
insights with automated machine learning techniques, implement-
ing advanced feature engineering from vulnerability descriptions,
temporal analysis, and vendor information. The system employs
multiple ML models (XGBoost, Random Forest, Neural Networks)
with comprehensive validation procedures.
Our results demonstrate that public data sources can provide mean-
ingful capabilities for vulnerability prediction. The Random Forest
model achieved an RMSE of 0.199 and an R2 score of 0.137, repre-
senting substantial improvement over baseline predictions. While
we processed 503 CVEs through manual collection, we identified po-
tential for 90,000+ CVEs through automated pipelines. Key insights
include the critical importance of automation in data collection and
the effectiveness of sophisticated feature engineering techniques.
This work successfully proves that vulnerability exploitation pre-
diction using public data is both feasible and valuable. We provide a
transparent, reproducible framework that democratizes vulnerabil-
ity risk assessment and enables community-driven innovation. The
research establishes ExploitDB[1] as a viable primary data source
and sets benchmarks for public-data-based exploitation prediction.
Although achieving a robust performance requires additional devel-
opment effort, this work provides a clear foundation for advancing
transparent cybersecurity prediction systems.
Keywords: Vulnerability Prediction, EPSS, Public Data, Machine
Learning, Transparency]

## 🤝 Contributing

This is a thesis project, but suggestions and improvements are welcome through issues and pull requests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- [Mubaraq M. Fuseini] - [Vrije Universiteit]
- [Almuthana Almustafa] - [Vrije Universiteit]
- [Abdalla Abdelhalik] - [Vrije Universiteit]


## 📞 Contact

For questions about this research, please contact: [vu.nl]

---

**Note**: This repository contains research code and may require additional setup for reproduction. Please refer to the thesis document for complete methodology and results interpretation. 