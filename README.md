# Student Depression Dataset - SQL & Tableau Analytics Project

![Status](https://img.shields.io/badge/Status-Active-brightgreen) ![Version](https://img.shields.io/badge/Version-1.0-blue) 

## 📊 Project Overview

This project presents a comprehensive analysis of student depression patterns through **interactive Tableau visualizations** combined with rigorous **SQL data cleaning and preprocessing**. The analysis explores the relationship between academic pressure, financial stress, sleep patterns, study hours, and study satisfaction among students.

## 🎯 Key Objectives

- **Data Cleaning**: SQL-based preprocessing including data modification, column updates, and validation
- **Exploratory Analysis**: Identify correlations between student lifestyle factors and depression indicators
- **Interactive Dashboard**: Create dynamic, filterable Tableau visualizations for stakeholder insights
- **Data Visualization**: Present complex relationships through intuitive, actionable charts

## 📁 Project Structure

```
student-depression-tableau-project/
├── README.md
├── sql/
│   ├── data_cleaning.sql          # Data preprocessing queries
│   ├── data_validation.sql        # Validation and integrity checks
│   └── sample_queries.sql         # Exploratory analysis queries
├── dataset/
│   ├── raw_data/                # Original dataset
├── tableau/
│   ├── Student-Depression-Dashboard.twbx  # Tableau workbook file
│   ├── visualizations/
│   │   ├── Academic_Pressure_Analysis.png
│   │   ├── Financial_Stress_Analysis.png
│   │   ├── Sleep_Duration_Analysis.png
│   │   ├── Study_Hours_Analysis.png
│   │   ├── Study_Satisfaction_Analysis.png
│   │   └── Dashboard_Overview.png
│   └── Student Depression Analysis.pdf   # Sheet PDF

```

## 🔍 Dashboard Features

### 5 Interactive Sheets + Master Dashboard

**1. Academic Pressure Analysis**
- Distributes student count across 5 academic pressure levels (AP-1 to AP-5)
- Shows correlation with depression indicators
- Filter-enabled visualization for multi-dimensional analysis

**2. Financial Stress Analysis**
- Breaks down student population by financial stress levels (FS-1 to FS-5)
- Highlights impact on mental health metrics
- Cross-filtered with other dimensions

**3. Sleep Duration Analysis**
- Categories: Less than 5 hours, 5-6 hours, 7-8 hours, More than 8 hours
- Visual representation of sleep patterns among depressed students
- Linked filter to dashboard controls

**4. Study Hours Analysis**
- Range distribution: 0-12 hours per day
- Density chart showing study time concentration
- Interactive filtering with other dimensions

**5. Study Satisfaction Analysis**
- Scale 1-5 satisfaction levels
- Correlation with depression outcomes
- Multi-level filtering capability

**Master Dashboard**
- Integrated view of all 5 sheets
- Synchronized filters for academic pressure, study hours, sleep duration, and financial stress
- Real-time cross-sheet filtering
- Action-based navigation for deep dives

## 🛠 Technical Stack

| Component | Technology | Version |
|-----------|-----------|---------|
| Data Cleaning | SQL | Standard SQL |
| Database | SQL Server | Latest |
| Visualization | Tableau Desktop | 2024.x |
| Hosting | Tableau Cloud | Production |
| Version Control | Git/GitHub | - |

## 📊 Data Cleaning & Preprocessing

### SQL Operations Performed

**Key Preprocessing Steps:**
- Removed NULL and duplicate values
- Standardized data formats across all columns
- Added calculated fields for depression indicators
- Validated data integrity and consistency
- Created indexing for performance optimization

## 📈 Key Findings

- **Academic Pressure Peak**: Level 3 shows the highest student count (11 students)
- **Sleep Deprivation**: 12 students sleep 5-6 hours, significantly higher than other categories
- **Study Hours Pattern**: Most students study 3-4 hours daily (53 and 46 students respectively)
- **Financial Stress**: Level 4 financial stress affects 10 students
- **Study Satisfaction**: Levels 4 and 2 have highest satisfaction counts (9 and 8 students)

## 🔗 Live Dashboard Links

- **Tableau Public**: [View Interactive Dashboard](https://public.tableau.com/views/YOUR-DASHBOARD-NAME)
- **Tableau Cloud**: [Production Dashboard](#) *(Internal access)*

## 💾 Data Dictionary

| Column Name | Data Type | Description |
|------------|-----------|-------------|
| Index | Integer | Unique student identifier |
| Academic_Pressure | Integer (1-5) | Level of academic pressure |
| Study_Hours | Integer (0-12) | Daily study hours |
| Sleep_Duration | String | Sleep duration category |
| Financial_Stress | Integer (1-5) | Financial stress level |
| Study_Satisfaction | Integer (1-5) | Satisfaction with study (1=Low, 5=High) |
| Depression | Binary/Integer | Depression indicator |

## 🚀 How to Use

### Accessing the Dashboard

1. **Interactive Version**: Visit Tableau Cloud link (requires account credentials)
2. **View Only**: Access Tableau Public for public viewing
3. **Local Tableau Desktop**: Download .twbx file and open in Tableau Desktop

### Filter Navigation

- **Academic Pressure Filter**: Adjust to view specific pressure levels
- **Study Hours Slider**: Select hour ranges to analyze
- **Sleep Duration Dropdown**: Filter by sleep category
- **Financial Stress Filter**: Compare stress levels
- All filters sync automatically across dashboard sheets

### Exporting Data

Use Tableau export functions to:
- Download visualizations as PNG/PDF
- Export data extracts for further analysis
- Generate PDF reports

## 📋 Prerequisites

To reproduce this analysis:

- **SQL Database**: MySQL, PostgreSQL, or SQL Server
- **Tableau Desktop**: Version 2024.x or latest
- **Git**: For cloning repository
- **Raw Dataset**: Student depression dataset (included in `/data/raw_data/`)

## 🔧 Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/student-depression-tableau-project.git
cd student-depression-tableau-project

# 2. Set up SQL database
# Import raw data into your SQL server
mysql -u root -p database_name < data/raw_data/student_data.sql

# 3. Run SQL cleaning scripts
mysql -u root -p database_name < sql/data_cleaning.sql

# 4. Connect Tableau to cleaned data
# Open Tableau Desktop → New Data Source → SQL Server/MySQL
# Point to cleaned_students table

# 5. Open Tableau workbook
# File → Open → tableau/Student-Depression-Dashboard.twbx
```

## 📸 Visualization Previews

See the `/tableau/visualizations/` folder for:
- Individual sheet screenshots (PNG format)
- Dashboard overview image
- Filter interaction examples
- Exported PDF reports

## 💡 Insights & Recommendations

1. **Stress Management**: Students with AP-3 and high financial stress need targeted interventions
2. **Sleep Optimization**: 7-8 hours sleep correlates with better mental health outcomes
3. **Study Balance**: Moderate study hours (4-6) show better satisfaction rates
4. **Holistic Approach**: Address multiple stressors simultaneously for effective depression prevention

## 🔐 Data Privacy

- All personal identifiers have been anonymized
- Index columns used for tracking instead of names
- Compliant with data protection standards
- Safe for academic and research publication

## 📚 SQL Scripts Included

| Script | Purpose |
|--------|---------|
| `data_cleaning.sql` | Primary data preprocessing and transformation |
| `data_validation.sql` | Quality checks and anomaly detection |
| `sample_queries.sql` | Exploratory queries for analysis |

## 🤝 Contributing

Suggestions for improvements:
- Additional statistical analysis
- Predictive modeling for depression risk
- Extended demographic analysis
- Performance optimization queries

## 📄 License

\

## 🙏 Acknowledgments

- Dataset source: [Student Depression Dataset on Kaggle/Source]
- Tableau community for best practices
- SQL optimization resources

## 📅 Project Timeline

| Phase | Date | Status |
|-------|------|--------|
| Data Collection | Oct 2025 | ✅ Complete |
| SQL Cleaning & Preprocessing | Oct 2025 | ✅ Complete |
| Tableau Dashboard Development | Nov 2025 | ✅ Complete |
| Cloud Deployment | Nov 2025 | ✅ Complete |
| Documentation | Nov 2025 | ✅ Complete |

## 🔄 Version History

- **v1.0** (Nov 16, 2025): Initial release with 5 sheets and master dashboard
- Coming soon: Predictive analytics module, Advanced filtering, Mobile optimization

---

**Last Updated**: November 16, 2025  
**Dashboard Status**: ✅ Active on Tableau Cloud  
**Data Last Refreshed**: November 15, 2025
