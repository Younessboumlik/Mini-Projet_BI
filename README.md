# Mini-Projet BI: Analyse de l’Impact et des Effets Indésirables d’un Médicament

## Description
This project implements a BI system to analyze the impact and side effects of medications. It leverages Microsoft tools such as SQL Server, SQL Server Integration Services (SSIS), SQL Server Analysis Services (SSAS), and Power BI to create a comprehensive decision-support system.

---

## Technical Environment
The following tools and technologies were used:
- **SQL Server** (Free or Full Edition): For relational database management.
- **SQL Server Integration Services (SSIS)**: For ETL pipeline creation.
- **SQL Server Analysis Services (SSAS)**: For OLAP cube modeling.
- **Power BI**: For data visualization and dashboard creation.

---

## Deliverables
1. **OLTP and Data Warehouse Models**:
   - OLTP Schema: Includes tables for medications, patients, side effects, and effectiveness.
  
     ![image](https://github.com/user-attachments/assets/0946a4c0-0e5b-4608-b63c-45771df49391)

   - DW Schema: Dimensional tables and fact tables for optimized querying.
  
     ![image](https://github.com/user-attachments/assets/a0e32d5d-576c-41fc-9103-1673eef50b9f)


   

2. **ETL Pipeline**:
   - SSIS package for extracting, transforming, and loading data.
   - Example transformations: Normalizing severity levels, categorizing patient age groups, and creating temporal hierarchies.

   ![image](https://github.com/user-attachments/assets/dbe9d865-f179-4981-bace-7e9ac224b959)

   ![image](https://github.com/user-attachments/assets/37e56513-7bb1-4170-9397-34a57fe56a0c)

   ![image](https://github.com/user-attachments/assets/c6f03f59-6edc-4626-89dc-109486e3d0f2)


   ![image](https://github.com/user-attachments/assets/accde20f-be79-469f-9d40-ec7ab5c10893)



4. **OLAP Cube**:
   - Multidimensional model with hierarchies for time, medications, and patients.
   - Measures like the count of reported effects and aggregated severity levels.

    ![image](https://github.com/user-attachments/assets/268b6efe-2cf3-4d5c-b10c-948f6cec73b0)

    ![image](https://github.com/user-attachments/assets/b7508879-df07-4d51-9b2e-78928b736d18)

    ![image](https://github.com/user-attachments/assets/8c84d0e9-cb06-40df-9dd7-50b66c7e1d61)

    ![image](https://github.com/user-attachments/assets/80c27a06-3627-4d76-9c7b-a7f07fa427da)

    ![image](https://github.com/user-attachments/assets/71733922-9b88-4b39-998f-5a92ee5bccaf)

   
5. **Interactive Power BI Dashboard**:
   - Bar charts showing adverse effects by therapeutic class.
   - Geographic maps displaying effects by patient regions.
   - KPIs such as the incidence rate of severe effects and clinical success rates.

    ![image](https://github.com/user-attachments/assets/63c2f202-93a2-487a-b4ab-6c4c62d6caee)

    ![image](https://github.com/user-attachments/assets/310ddb7d-b5a0-4547-acf3-1b053721c4f8)

   ![image](https://github.com/user-attachments/assets/973764cc-3f5c-4b06-864c-0b79b08ff4c8)

   ![image](https://github.com/user-attachments/assets/d7c8eb7c-466d-4549-9095-2d6cbddb7650)


    ![image](https://github.com/user-attachments/assets/6ca9e9d1-afe6-4b1a-98e3-f2b9f460c320)


---

## Project Steps

### 1. Database Creation (OLTP)
- Designed and populated the `Medi_DB` operational database with:
  - Medications table.
  - Patients table.
  - Side effects table.
  - Effectiveness table.

### 2. Data Warehouse Design (DW)
- Schema includes:
  - **Dimensions**: Medications, Patients, and Time.
  - **Fact Table**: Aggregated side effect data.

### 3. ETL Implementation
- Created a data pipeline in SSIS to:
  - Extract data from the OLTP database.
  - Apply transformations (e.g., severity normalization, age categorization).
  - Load data into the DW schema.

### 4. OLAP Cube Development
- Modeled dimensions and measures in SSAS.
- Deployed and processed the cube to enable multidimensional analysis.

### 5. Visualization with Power BI
- Connected to the SSAS cube to create:
  - Interactive dashboards with KPIs, charts, and maps.
  - Published reports with automated alerts.

[View the Power BI Dashboard](https://app.powerbi.com/groups/me/reports/d8ad7378-06d6-4dd0-bf07-01e2a08c58a5/3b5ea353af924e6013ce?experience=power-bi)


---

## Usage Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/Younessboumlik/Mini-Projet_BI
   ```
2. Follow the project steps to set up the database, ETL pipeline, OLAP cube, and dashboards.

---

## Acknowledgments
This project was completed as part of the **Systèmes d’aide à la décision** module at **Ecole Nationale des Sciences Appliquées de Khouribga** under the guidance of **Prof. Mostafa SAADI**.

--- 
