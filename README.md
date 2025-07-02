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
├── code-5/
│   ├── 31xxx/                    # CVE JSON files (160+ records)
│   ├── EPSS.ipynb               # EPSS data processing
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
git clone https://github.com/yourusername/cve-risk-assessment-thesis.git
cd cve-risk-assessment-thesis

# Install dependencies
pip install -r code-5/requirements.txt

# Start Jupyter
jupyter notebook
```

### Usage
1. Open `code-5/Init.ipynb` to set up the environment
2. Run `code-5/EPSS.ipynb` to process EPSS data
3. Execute `code-5/Mubaraq.ipynb` for the main analysis

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

This code accompanies our thesis: **[Thesis Title]** by [Your Names]

**Abstract**: [Brief abstract of your thesis]

## 🤝 Contributing

This is a thesis project, but suggestions and improvements are welcome through issues and pull requests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- [Your Name] - [Your Institution]
- [Co-author Name] - [Institution]

## 📞 Contact

For questions about this research, please contact: [your.email@institution.edu]

---

**Note**: This repository contains research code and may require additional setup for reproduction. Please refer to the thesis document for complete methodology and results interpretation. 