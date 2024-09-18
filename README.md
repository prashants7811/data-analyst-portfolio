# Projects

Overview of the projects

---

## **Project 1: Exploratory Data Analysis for Prior Learning Recognition Trends Analysis**

### **Project Title**:
**Enrollment and Prior Learning Recognition Trends Analysis at University Canada West (UCW) Using AWS**

### **Project Description**:
This project focuses on performing an Exploratory Data Analysis (EDA) of the Prior Learning Assessment and Recognition (PLAR) and Enrollment dataset from UCW. The analysis explores trends in student enrollment, prior learning recognition, program distribution, and retention rates. By utilizing AWS services like S3, Glue, and Athena, the project identifies key trends from student demographics, recognition outcomes, and program participation, providing valuable insights for academic decision-making.

### **Dataset**:
The dataset contains the following fields:
- **StudentID**: Unique identifier for each student.
- **FirstName**: First name of the student.
- **LastName**: Last name of the student.
- **DateOfBirth**: Date of birth of the student.
- **Gender**: Gender of the student.
- **Program**: Academic program of enrollment (e.g., MBA, BCom).
- **EnrollmentDate**: Date of enrollment.
- **RecognitionType**: Type of prior learning recognition (e.g., Work Experience, Certification).
- **RecognitionOutcome**: Status of recognition (Approved/Denied).
- **ExpectedGraduationDate**: Expected graduation date.
- **Status**: Enrollment status (Enrolled/Graduated).

### **Objective**:
To analyze student enrollment trends and the recognition of prior learning using AWS services, with the goal of identifying patterns in student demographics, program participation, and the overall impact on graduation and retention rates.

### **Methodology**:

1. **Data Collection and Preparation**:
   - **Data Storage**: Uploaded the dataset to an Amazon S3 bucket for secure storage.
   - **Data Cleaning and Transformation**: 
     - Created an ETL pipeline in AWS Glue to clean the dataset, handle missing values, and format dates (DateOfBirth, EnrollmentDate).
     - Converted the dataset to a queryable format (Parquet) to optimize performance.
   - **AWS Glue Catalog**: Managed metadata using AWS Glue Catalog for efficient querying.

2. **Descriptive Statistics**:
   - Used AWS Athena to run SQL queries, generating summary statistics:
     - Calculated the average student age based on DateOfBirth.
     - Counted students per program and recognition outcome.
     - Analyzed the distribution of enrollment dates and recognition outcomes across programs.

3. **Data Visualization**:
   - **Amazon QuickSight** for interactive data visualization:
     - **Bar Charts**: Displayed student counts across academic programs and recognition outcomes.
     - **Pie Charts**: Visualized the gender distribution of students applying for prior learning recognition.
     - **Line Charts**: Showed enrollment and recognition trends over time.
     - **Stacked Bar Charts**: Explored program-wise gender distribution and recognition trends.

4. **Recognition and Graduation Trends Analysis**:
   - Used Athena for further analysis:
     - Identified programs with higher recognition approval rates.
     - Analyzed gender-based patterns in recognition approvals and graduation rates.
     - Tracked year-over-year changes in enrollment and recognition outcomes.

5. **Insights and Findings**:
   - **Recognition Trends**: Programs like the MBA showed higher recognition approval rates.
   - **Gender Patterns**: Gender-based trends revealed differences in recognition applications.
   - **Enrollment Growth**: Noted trends in enrollment and recognition growth over time, providing insights for academic planning.

### **Tools and Technologies**:
- **AWS S3**: Data storage.
- **AWS Glue**: Data cleaning, transformation, and cataloging.
- **AWS Athena**: SQL querying and analysis.
- **Amazon QuickSight**: Data visualization.

### **Deliverables**:
- AWS Glue ETL pipeline code.
- SQL queries executed in AWS Athena.
- A presentation summarizing insights and findings for university stakeholders.

---

## Project 2: Descriptive Analysis of Vancouver Business License Issuances

### **Project Title:**
Descriptive Analysis of Vancouver Business License Issuances (2023-2024) Using AWS

### **Project Overview:**
This project focuses on analyzing business licenses issued in Vancouver between 2023 and 2024. The objective is to extract insights into the types of businesses, timelines for license issuance, fees, and trends influencing Vancouver's business ecosystem. The analysis is powered by AWS services such as **S3** for data storage, **Glue** for ETL processes, **Athena** for querying, and **QuickSight** for visualization, enabling actionable insights and informed decision-making.

### **Dataset:**
Key features of the dataset include:
- **LicenseNumber**: Unique identifier for each business license.
- **BusinessName**: Name of the business receiving the license.
- **IssueDate**: Date the business license was issued.
- **BusinessType**: Type of business (e.g., Retail, Restaurant, Services).
- **LicenseFee**: Amount paid for the license.
- **LicenseStatus**: Status of the license (e.g., Active, Expired).
- **Address**: Business location.
- **LicenseCategory**: Category of the business (e.g., Commercial, Residential, Industrial).
- **IssueYear**: Year the license was issued.
- **GeoLocalArea**: Geographic region within Vancouver.

### **Objective:**
The goal of this project is to conduct a descriptive analysis of business license issuance in Vancouver. The insights help in understanding business growth, fee structures, common business types, and geographic trends, supporting city planning and economic strategy decisions.

### **Methodology:**

#### 1. **Data Ingestion:**
   - Ingest the business license dataset into **Amazon S3** in CSV format for scalable, secure storage.

#### 2. **Data Cleaning and Transformation:**
   - Use **AWS Glue** to clean and transform data, including:
     - Parsing date fields to track license issuance timelines.
     - Standardizing business types and calculating fees.
     - Adding metrics like the average time between application and issuance.

#### 3. **Data Querying:**
   - **AWS Athena** is employed to query the cleaned data using SQL to derive insights such as:
     - Average license fees categorized by business type and geographic region.
     - License issuance timelines and trends over time.
     - Most common types of businesses receiving licenses.
     - Geographic distribution of high-fee business licenses.

#### 4. **Data Visualization:**
   - **AWS QuickSight** is used to create visualizations, including:
     - **License Fees Over Time**: Time-series analysis showing fluctuations in fees.
     - **Geographic Heatmaps**: Visualizing concentrations of licenses issued across Vancouver.
     - **Business Type Distribution**: Bar charts depicting the breakdown of businesses by type and category.

### **Insights and Findings:**
- **License Trends**: Insight into average fees by business type, common license categories, and active geographic areas.
- **High-Fee Licenses**: Identification of high-fee licenses and their geographic concentrations.
- **Business Growth**: Seasonal trends in business license issuance and emerging business hotspots across Vancouver.

### **Tools and Technologies:**
- **Amazon S3**: Scalable, secure data storage.
- **AWS Glue**: ETL processes for cleaning, transforming, and categorizing data.
- **Amazon Athena**: SQL querying for structured datasets.
- **AWS QuickSight**: Creating interactive dashboards and visualizations.

### **Deliverables:**
- **Detailed Report**: Summarizing insights, trends, and findings from the analysis.
- **AWS QuickSight Visualizations**: Interactive dashboards showcasing key metrics such as business types, fee structures, and geographic trends.
- **Presentation**: A comprehensive presentation to stakeholders, emphasizing trends useful for city planning and business development.

### **Timeline:**
- **Week 1-2**: Data ingestion and cleaning with **AWS Glue**.
- **Week 3**: Data querying and analysis using **AWS Athena**.
- **Week 4**: Visualization creation with **AWS QuickSight**.
- **Week 5**: Report generation and presentation preparation.

---

## Project 3: Diagnostic Analysis Using AWS Services

## **Project Title**  
**Diagnostic Analysis of Vancouver Business License Issuances (2023-2024) Using AWS**

### **Project Overview**  
This project focuses on diagnostic analysis of business licenses issued in Vancouver during 2023 and 2024. The analysis uncovers insights into factors influencing license issuance, including processing timelines, geographic concentration of businesses, business types, and fee structures. Using AWS services—S3 for data storage, Glue for cleaning, Athena for querying, and QuickSight for visualizations—the project identifies bottlenecks and business opportunities in Vancouver's licensing process.

### **Objective**  
The objective is to analyze business license issuance data from Vancouver (2023-2024), identifying trends and bottlenecks related to processing times, license fees, business types, and geographic areas. This analysis will support city officials and business developers in optimizing the licensing process and recognizing high-growth business areas.

### **Dataset**  
Key features of the dataset include:  
- **LicenseNumber**: Unique identifier for each license  
- **BusinessName**: Name of the licensed business  
- **LicenseFee**: Fee paid for the license  
- **IssueDate**: Date of license issuance  
- **ProcessingTime**: Days between application and issuance  
- **BusinessType**: Type of business (e.g., Retail, Restaurant)  
- **LicenseStatus**: License status (e.g., Active, Expired)  
- **GeoLocalArea**: Geographical area within Vancouver  

### **Methodology**  

#### **1. Data Collection and Preparation**  
- **Data Storage**: The dataset is consolidated and stored in Amazon S3.  
- **Data Cleaning**: AWS Glue is used for cleaning, handling missing values, and standardizing fields (LicenseFee, BusinessType, GeoLocalArea).

#### **2. Diagnostic Analysis Using AWS Athena**  
- **Queries**: Athena is used for diagnostic queries to analyze:  
  - Average processing time by business type and region  
  - Geographic distribution of businesses with varying processing times  
  - Correlation between license fees and processing times  
  - Identification of bottlenecks in the process for specific business types or regions

#### **3. Trend Analysis**  
- **License Processing Times**: Analyze trends over two years by business type and region.  
- **Fee Analysis**: Identify relationships between fees and processing times.  
- **Geospatial Analysis**: Map delays in license issuance across Vancouver using Athena and QuickSight.

#### **4. Data Visualization**  
- **Visualizations in QuickSight**:  
  - **Heatmaps**: Map business license processing times across Vancouver.  
  - **Bar Charts**: Compare average processing times by business type across years.  
  - **Scatter Plots**: Visualize correlations between license fees and processing times.

### **Insights and Findings**  
- **Bottleneck Identification**: Some business types (e.g., restaurants) experience longer processing times, indicating inefficiencies.  
- **Geographic Trends**: Certain areas face delays, potentially due to regulatory or density-related challenges.  
- **Fee-to-Time Relationship**: Higher fees may not always correspond to quicker processing, presenting opportunities for optimization.

### **Tools and Technologies**  
- **Amazon S3**: For scalable data storage  
- **AWS Glue**: For ETL, data cleaning, and transformation  
- **Amazon Athena**: For querying and running diagnostic analyses  
- **AWS QuickSight**: For visualizing diagnostic trends and insights  

### **Deliverables**  
- **Diagnostic Report**: A detailed report of key findings, bottlenecks, and trends  
- **Visual Dashboards**: Interactive dashboards showcasing processing times, geographic trends, and correlations  
- **Recommendations**: Actionable insights to improve licensing efficiency and identify business opportunities  

### **Timeline**  
- **Week 1-2**: Data ingestion, cleaning, and normalization with AWS Glue  
- **Week 3**: Diagnostic analysis with AWS Athena  
- **Week 4**: Visualization and reporting using AWS QuickSight  
- **Week 5**: Finalization and presentation of the report to stakeholders  

---

## Project 4: Data Wrangling for University Enrollment Analysis Using AWS Services

### **Project Title**  
**Data Wrangling of University Canada West (UCW) Enrollment and Prior Learning Assessment Data Using AWS**

### **Project Overview**  
This project involves performing comprehensive data wrangling on the University Canada West (UCW) student enrollment and Prior Learning Assessment and Recognition (PLAR) dataset. The goal is to clean, transform, and prepare the dataset for further analysis and reporting. AWS services such as S3 for data storage, Glue for ETL, and Athena for querying were utilized to facilitate deeper analysis into enrollment trends, prior learning recognition outcomes, and program distribution. This wrangled data will aid UCW in enhancing its decision-making capabilities regarding student retention, program development, and academic progress tracking.

### **Objective**  
The primary objective of this project is to conduct comprehensive data wrangling on UCW’s enrollment and PLAR dataset. By cleaning and transforming the data, the goal is to enhance the dataset’s accuracy and usability for descriptive and diagnostic analysis of student enrollment patterns, recognition trends, and demographics. This process will enable UCW to gain actionable insights for optimizing academic programs and improving student retention strategies.

### **Dataset**  
Key features of the dataset include:  
- **StudentID**: Unique identifier for each student  
- **FirstName, LastName**: Name of the students  
- **DateOfBirth**: Birthdate of the students  
- **Gender**: Gender of the students  
- **Program**: Academic program of the student  
- **EnrollmentDate**: Date the student enrolled  
- **ExpectedGraduationDate**: The expected graduation date  
- **RecognitionType**: Type of prior learning recognition (e.g., Work Experience, Certification)  
- **RecognitionOutcome**: Status of the recognition (Approved/Denied)  
- **Status**: Enrollment status (Enrolled/Graduated)  
- **Email**: Contact email of the students  

### **Methodology**  

#### **1. Data Ingestion**  
- The dataset is ingested and stored securely in Amazon S3 in CSV format for scalable storage and retrieval.

#### **2. Data Cleaning and Transformation Using AWS Glue**  
- **Data Cleaning**: AWS Glue is used to clean the dataset by:
  - Parsing and formatting date fields (DateOfBirth, EnrollmentDate, ExpectedGraduationDate)
  - Standardizing gender entries (e.g., “M/F”)
  - Normalizing recognition status fields (e.g., Approved/Denied)
  - Handling missing values and ensuring consistency across fields
- **Data Transformation**: Additional metrics calculated include:
  - **EnrollmentDuration**: Difference between EnrollmentDate and ExpectedGraduationDate  
  - **RecognitionRate**: Proportion of students who received prior learning recognition

#### **3. Data Querying Using AWS Athena**  
- Amazon Athena is used to run SQL queries on the cleaned dataset to:
  - Analyze student distribution across programs and recognition types
  - Track enrollment trends over time by gender, program, and year  
  - Identify patterns in prior learning recognition outcomes  
  - Calculate average graduation timelines and program completion rates

#### **4. Data Visualization**  
- **AWS QuickSight**: Interactive dashboards created to visualize:
  - **Enrollment Trends**: Display student enrollment trends by year and program  
  - **Gender Distribution**: Analyze gender representation across programs  
  - **Recognition Outcomes**: Show trends in recognition outcomes by program  
  - **Graduation Timelines**: Track average time-to-graduation across programs  

### **Wrangling Process**  

#### **1. Discover**  
- Conducted an initial assessment to understand data structure, types, and quality.
- Performed Exploratory Data Analysis (EDA) to detect missing values, anomalies, and outliers.

#### **2. Structure**  
- Defined schemas and data types for each field, ensuring consistent formatting for dates, numerical fields, and categorical variables.

#### **3. Clean**  
- Managed missing values through imputation or removal of incomplete records.
- Removed duplicate entries using StudentID as a key.
- Corrected errors in program names, status fields, and other inconsistencies.

#### **4. Enrich**  
- **Feature Engineering**: Calculated EnrollmentDuration and derived Age from DateOfBirth.  
- Standardized categorical variables (Gender, Status, Program) for analysis.

#### **5. Validate**  
- Ensured data consistency by checking logical relationships (e.g., EnrollmentDate precedes GraduationDate).
- Conducted quality assurance to ensure data transformations maintained integrity.

#### **6. Publish**  
- Stored the cleaned and enriched dataset in Amazon S3 for further analysis.  
- Documented all data wrangling steps, transformations, and insights for reproducibility.

### **Tools and Technologies**  
- **Amazon S3**: Scalable data storage  
- **AWS Glue**: Data cleaning, transformation, and ETL processes  
- **Amazon Athena**: SQL-based querying for analytics  
- **AWS QuickSight**: Visualization of insights and trends  
- **AWS EC2**: Scalable compute resources for data processing  
- **AWS VPC**: Secure environment for EC2 instances  

### **Deliverables**  
- **Cleaned Dataset**: CSV format dataset cleaned and transformed for analysis  
- **Data Wrangling Report**: Comprehensive documentation of the cleaning and transformation process  
- **Interactive Dashboards**: AWS QuickSight dashboards highlighting key insights such as enrollment trends, gender distribution, and graduation timelines  

### **Timeline**  
- **Week 1-2**: Data ingestion and discovery phase  
- **Week 3**: Data structuring and cleaning using AWS Glue  
- **Week 4**: Data enrichment and validation  
- **Week 5**: Data querying and analysis with Amazon Athena  
- **Week 6**: Visualization creation with AWS QuickSight  
- **Week 7**: Compilation of final documentation and reports  
- **Week 8**: Presentation and project handover  

---

## Project 5: Data Quality Control Analysis for Vancouver Business Licenses Using AWS Services

### Project Title:
**Data Quality Control Analysis of Vancouver Business License Issuances (2023-2024) Using AWS**

### Project Overview:
This project focuses on performing a **data quality control analysis** of business licenses issued in Vancouver between **2023 and 2024**. The goal is to ensure the **quality and consistency** of the dataset by implementing data quality checks during the ETL process using **AWS Glue**. **AWS Athena** is used for querying, while **AWS QuickSight** visualizes trends and data quality metrics. This analysis helps inform the **City of Vancouver** on improvements in data management, ensuring **data integrity** for future decision-making.

### Objectives:
1. Perform **ETL (Extract, Transform, Load)** on Vancouver’s business license dataset using AWS services.
2. Ensure the dataset meets **predefined quality standards** such as completeness, accuracy, and consistency.
3. Visualize trends in license issuance to support business development strategies in Vancouver.
4. Monitor and control ongoing data quality using AWS tools.

### Dataset Features:
- **LicenseNumber**: Unique identifier for each business license.
- **BusinessName**: Name of the business.
- **IssueDate**: Date the license was issued.
- **BusinessType**: Type of business (e.g., Retail, Restaurant).
- **LicenseFee**: Fee paid for the license.
- **LicenseStatus**: Status of the license (Active, Expired).
- **GeoLocalArea**: Geographic region within Vancouver.
- **Address**: Business location.

### Methodology:

#### 1. Data Ingestion:
- **Data Source**: Vancouver’s open data platform.
- **AWS S3**: Dataset uploaded in CSV format for secure storage.

#### 2. Data Cleaning and Transformation Using AWS Glue:
- **ETL Pipeline**: AWS Glue used to build the ETL pipeline.
- **Data Cleaning**: 
  - Handle missing/erroneous data.
  - Parse date fields (e.g., IssueDate).
  - Standardize business types and address formats.
- **Data Quality Metrics**:
  - **Completeness**: Ensure 95% of critical fields are populated.
  - **Uniqueness**: Remove duplicates to maintain 90% uniqueness for LicenseNumber.
  - **Consistency**: Standardize business types and verify geographic accuracy.

#### 3. Data Quality Control Using AWS Glue and Athena:
- **Data Governance**: Implement compliance with **PIPEDA**.
- **Validation Checks**: 
  - Validate license fees across business types.
  - Ensure issue dates align with business categories.
- **AWS Athena**: Execute SQL queries for data validation and to check discrepancies in fields like **LicenseFee** and **GeoLocalArea**.

#### 4. Data Visualization Using AWS QuickSight:
- **Interactive Dashboards**:
  - **Data Completeness**: Bar charts showing percentage of missing/incomplete data.
  - **Geographic Accuracy**: Maps displaying business license distributions.
  - **License Fee Trends**: Visualize anomalies or outliers in license fees across business types.

### Insights and Findings:
- **Data Completeness**: Identified fields with significant missing data, highlighting potential issues in data entry.
- **Data Consistency**: Standardizing business types and verifying geographic data improved dataset reliability.
- **Geographic Trends**: Geographic distributions identified regions with poor data quality due to inconsistent entry practices.

### Tools and Technologies:
- **AWS S3**: Scalable data storage.
- **AWS Glue**: Data cleaning, transformation, and quality control.
- **AWS Athena**: Querying the dataset for quality checks.
- **AWS QuickSight**: Data visualization and interactive dashboards.
- **AWS CloudWatch**: Monitoring ETL performance and tracking data quality.
- **AWS CloudTrail**: Auditing changes and interactions with the data pipeline for compliance.

### Deliverables:
- **Data Quality Control Plan**: Document outlining quality checks and metrics.
- **Cleaned and Validated Dataset**: High-quality data ready for further analysis.
- **Interactive Dashboards**: AWS QuickSight dashboards for real-time data quality tracking.
- **Reports and Recommendations**: Summarized findings and suggestions for improving data entry and management.

### Timeline:
- **Week 1-2**: Data ingestion and quality assessment.
- **Week 3-4**: Data cleaning and validation using AWS Glue and Athena.
- **Week 5**: Visualization creation using AWS QuickSight.
- **Week 6**: Reporting and presentation of findings to stakeholders.

