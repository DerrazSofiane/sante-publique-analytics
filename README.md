# Santé Publique Analytics 🏥

## OpenClassrooms Project 3: Public Health Data Engineering

### 📋 Project Overview
This project focuses on preparing and analyzing public health data for epidemiological studies. Working with global nutrition data from the FAO (Food and Agriculture Organization), the goal is to build a robust data pipeline that enables public health insights while ensuring data quality and privacy compliance.

### 🎯 Objectives
- Clean and prepare complex public health datasets
- Build ETL pipelines for epidemiological analysis
- Ensure GDPR compliance and data privacy
- Identify global malnutrition patterns
- Create reproducible data workflows

### 📊 Dataset
- **Source**: FAO (Food and Agriculture Organization) databases
- **Scope**: Global nutrition and food security data
- **Features**: 
  - Food availability by country
  - Nutritional indicators
  - Population demographics
  - Agricultural production data
- **Time Period**: Multiple years of historical data

### 🛠️ Technical Stack
- **Python 3.x**
- **Data Engineering**:
  - pandas - Data manipulation
  - numpy - Numerical computations
  - Apache Spark - Large-scale data processing
  - SQL - Database queries
- **Pipeline Orchestration**:
  - Apache Airflow (planned)
  - Docker - Containerization
- **Data Quality**:
  - Great Expectations
  - Custom validation scripts

### 📁 Repository Structure
```
sante-publique-analytics/
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_pipeline_development.ipynb
│   └── 04_analysis_results.ipynb
├── src/
│   ├── etl/
│   │   ├── extract.py
│   │   ├── transform.py
│   │   └── load.py
│   └── utils/
│       ├── data_quality.py
│       └── privacy_utils.py
├── config/
│   └── pipeline_config.yaml
├── tests/
├── requirements.txt
└── README.md
```

### 🔧 Data Pipeline Architecture

#### 1. Extraction Phase
```python
# Multiple data sources
- FAO statistical databases
- World Bank indicators
- WHO nutrition data
```

#### 2. Transformation Phase
- Data standardization across sources
- Missing value imputation strategies
- Outlier detection and handling
- Feature engineering for analysis

#### 3. Loading Phase
- Structured data warehouse design
- Optimized for analytical queries
- Partitioning strategies for performance

### 🔒 Privacy & Compliance

#### GDPR Compliance
- Anonymization techniques implemented
- Data minimization principles
- Audit trails for data access
- Right to erasure capabilities

#### Data Security
```python
# Encryption at rest and in transit
# Access control implementation
# Sensitive data masking
```

### 📊 Key Analyses

1. **Malnutrition Patterns**
   - Geographic distribution
   - Temporal trends
   - Correlation with economic indicators

2. **Food Security Metrics**
   - Availability vs. accessibility
   - Dietary diversity indices
   - Vulnerability assessments

3. **Predictive Models**
   - Risk factor identification
   - Early warning systems
   - Resource allocation optimization

### 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/DerrazSofiane/sante-publique-analytics.git
   ```

2. Set up environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Configure data sources:
   ```bash
   # Edit config/pipeline_config.yaml with your data paths
   ```

4. Run the pipeline:
   ```bash
   python src/run_pipeline.py
   ```

5. Explore results:
   ```bash
   jupyter notebook notebooks/04_analysis_results.ipynb
   ```

### 📈 Data Quality Metrics
- **Completeness**: 95%+ after cleaning
- **Consistency**: Cross-source validation
- **Timeliness**: Automated updates
- **Accuracy**: Validated against WHO standards

### 💡 Key Insights Generated
- Identification of high-risk regions
- Seasonal pattern detection
- Policy intervention effectiveness
- Resource allocation recommendations

### 🔄 Pipeline Features
- **Incremental Processing**: Only new/changed data
- **Error Handling**: Graceful failure recovery
- **Monitoring**: Data quality dashboards
- **Scalability**: Spark for large datasets

### 📝 Skills Demonstrated
- Data Engineering
- ETL Pipeline Development
- Big Data Processing (Spark)
- Data Privacy & Compliance
- Public Health Analytics
- Data Quality Management

### 🚀 Future Enhancements
- Real-time data streaming
- Machine learning predictions
- Interactive dashboards
- API for data access
- Automated reporting

### 🌍 Impact
- Supports evidence-based policy making
- Enables targeted interventions
- Improves resource allocation
- Facilitates international cooperation

### 📚 Documentation
- Detailed pipeline documentation in `/docs`
- Data dictionary available
- Privacy impact assessment included

### 🤝 Contact
Created by Sofiane Derraz as part of the OpenClassrooms AI Engineer certification program.

---
*Note: This educational project demonstrates data engineering best practices for sensitive health data. The methodologies are applicable to real-world public health surveillance and epidemiological research systems.*
