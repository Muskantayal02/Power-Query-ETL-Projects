**PROJECT OVERVIEW:**

This repository showcases multiple **ETL (Extract, Transform, Load)** projects demonstrating my end-to-end capability in data transformation, validation, and automation using **Microsoft Power Query**.

Each project demonstrates how real-world data challenges - from messy Excel sheets to combining datasets across files - can be solved through systematic data cleaning, transformation, and automation techniques.

These highlight, different Power Query capabilities - from basic cleaning to advanced joins, appends, and dynamic folder consolidation. It includes multiple data cleaning and reporting scenarios showing how to extract, transform, and load data efficiently for analysis and reporting.

All project outputs are consolidated in one Excel workbook:
**`PowerQuery_ETL_Projects.xlsx`**

Every sheet in the compiled workbook represents a standalone case study designed to highlight a specific Power Query capability such as data cleaning, merging, appending, and dynamic folder automation.

**SKILLS DEMONSTRATED**
- Power Query ETL (Extract, Transform, Load)
- Data Cleaning, Transformation & Structuring
- Data Appending, Merging & Filtering
- Working with Multiple Excel Files
- Web Scraping and Unpivoting
- Advanced Data Preparation for Reporting
- Automation using Connection-Only Queries
- Data Validation and Type Handling
- Business-Ready Data Modeling
&nbsp;

**PROJECT SUMMARIES**

**A) Employee Data Cleanup:** (_Sheet Name - Employee Data Cleaning_)

**Goal:** Clean and prepare HR dataset for reporting.

**Steps:**
* Removed extra rows/columns, promoted headers, and handled nulls.
* Replaced missing gender and department values with defaults.
* Extracted country from location column using “Column from Examples”.
* Standardized departments and filtered out ex-employee
* Converted data types for salary (currency) and date.

<img width="1920" height="1080" alt="1  EmployeeData_AppliedSteps" src="https://github.com/user-attachments/assets/68da0984-e921-459b-8093-69b8e6719509" />

&nbsp;

**Outcome:** Cleaned employee dataset ready for dashboard/reporting.

**Skills:** Data cleaning, type transformation, text extraction.

&nbsp;

**B) Web Scraping - India Population Data**  (_Sheet Name - India Population Web_)

**Goal:** Transform a messy web dataset into a structured table.

**Steps:**
* Connected to HTML table via Get Data → From Web.
* Removed unnecessary rows and columns, promoted headers
* Unpivoted year columns to normalize the data and reshape into tidy format.
* Extracted year values using Text Between Delimiters.
* Cleaned NA values, removed errors, and ensured standardized column types

&nbsp;

<img width="1920" height="1080" alt="2  WebScraping_Unpivot" src="https://github.com/user-attachments/assets/d477b82f-30d8-46fd-b5df-9dcbd1aeec02" />
&nbsp;

**Outcome:** A long-format dataset for population trends by state and year.

**Skills:** Web data extraction, Web connector, unpivoting, string parsing, data validation.

&nbsp;

**C) Excel Files Consolidation**  (_Sheet Name - Projects Consolidation_)

**Goal:** Combine monthly project data from multiple Excel files into one master table.

**Steps:**
* Connected to folder path and combined data using Combine & Transform.
* Transformed sample file, standardized project names (project-alpha.xlsx → project-alpha).
* Added a custom column to convert month numbers into date values using a formula =#date(2025, [Month],1)
* Filtered only .xlsx extensions files, changed types, and loaded final dataset
* Tested automation by adding a new file and refreshing queries successfully

&nbsp;

 <img width="1920" height="1080" alt="3  FolderConsolidation_Transform" src="https://github.com/user-attachments/assets/684082bc-cfe3-4d59-b488-1598bc8111e3" />
&nbsp;

**Outcome:** An automated consolidated project database that refreshes on new file addition.

&nbsp;

**Automation for New files**
&nbsp;

**_Initial files:_**
&nbsp;

<img width="1920" height="1080" alt="Screenshot (602)" src="https://github.com/user-attachments/assets/5c033584-8dc3-4c99-b506-cc3d96d53c80" />
&nbsp;

**_New File added:_**

&nbsp;
<img width="1920" height="1080" alt="Screenshot (603)" src="https://github.com/user-attachments/assets/ce741c75-917e-4da0-9d2c-f8426d8b5b2e" />
&nbsp;

**_Refreshed Output(Automated):_**
&nbsp;

<img width="1920" height="1080" alt="Screenshot (606)" src="https://github.com/user-attachments/assets/473ea624-e48b-4224-9702-b35cc6e162db" />

&nbsp;

**Skills:** Folder automation, dynamic ETL, custom column formulas, refresh testing.

&nbsp;

**D) Students & Courses (Append and Merge)**  (_Sheet Name - Female Students_)

**Goal:** Combine data from multiple classes and enrich it with course-level details.

**Steps:**
* Imported Year 11 and Year 12 student data, and added custom “Year” columns
* Appended both tables to create a single student dataset
* Merged with Course table (teacher, credits, assessment type) on Course field using Left Outer Join.
* Expanded course details (teacher, credits, assessment type).
  &nbsp;
<img width="1920" height="1080" alt="4  StudentCourse_Append_Merge" src="https://github.com/user-attachments/assets/c9c413fd-18de-4878-928b-b6e260318249" />

&nbsp;

**Outcome:** Unified student-course dataset ready for analytics and academic reporting.

**Skills:** Append queries, merge queries, relational data integration, reference queries, connection only.

&nbsp;

**E) Filtering Female Students on ≥3 Courses** (_Sheet Name - Female Students_)

**Goal:** Identify and analyze high-performing female students across multiple courses.

**Steps:**
* Created a reference query from the unified student dataset
* Filtered Gender = Female
* Applied filter for Credits ≥ 3
* Customized load behavior (set support tables as connection-only)
&nbsp;

<img width="1920" height="1080" alt="5  FemaleStudents_Filter" src="https://github.com/user-attachments/assets/f9757edb-beb9-4168-bab4-1096832d7056" />
&nbsp;

**Outcome:** A filtered, query-based insight table highlighting targeted academic groups.

**Skills:** Query referencing, load optimization, conditional filtering.
&nbsp;

**DELIVERABLES**

- **Excel Workbook:** `PowerQuery_ETL_Projects.xlsx` (contains all project sheets)
- **Transformation Screenshots:** Embedded in README below each project section.
&nbsp;

**KEY HIGHLIGHTS**

- Combined **5 distinct Power Query projects** demonstrating versatile ETL capabilities
- Used **Append**, **Merge**, **Unpivot**, **Custom Columns**, **Replace Values**, and **Connection-only Queries**
- Optimized query groups and loading behavior for performance
- Demonstrated both **one-time cleaning* and *refresh-based automation** workflows
- Showcases proficiency across **data preparation, transformation, and integration**
&nbsp;

**TECH STACK**

| Tool                               | Purpose                                         |
| ---------------------------------- | ----------------------------------------------- |
| **Microsoft Excel (Power Query)**  | Data extraction, transformation, and automation |

| Category | Tools / Skills |
|-----------|----------------|
| **Data Extraction & Cleaning** | Excel Power Query, ETL Techniques |
| **Data Modeling** | Power Pivot, Data Relationships |
| **Transformation Logic** | Merge Queries, Append Queries, Conditional Columns |
| **Automation & Formulas** | Dynamic Ranges, Named Tables |
| **Data Analysis** | Pivot Tables, Aggregation, Filtering |
| **Documentation** | Excel Comments, Step Annotations |
| **Conceptual Understanding** | SQL Joins (theory), Data Integrity Checks |
| **Data Sources** | Excel files, Web HTML tables |
| **Output** | Clean Excel datasets and summary pivot reports |


&nbsp;

**OUTCOME**

- This project demonstrates hands-on data preparation proficiency using Power Query — efficiently cleaning, merging, and automating data pipelines.
- It reflects analytical and technical ability to transform raw, unstructured data into structured, decision-ready outputs for analysis and reporting.


&nbsp;

**FUTURE ENHANCEMENTS**

* Link outputs to Power BI dashboards for visualization.
* Integrate data refresh automation with OneDrive or Power Automate.
* Add error-handling and dynamic parameterization for folders and URLs.
&nbsp;

**How to Use**

- Clone or download this repository.
- Open PowerQuery_ETL_Projects.xlsx in Excel (ensure Power Query is enabled).
- Go to Data → Queries & Connections → Refresh All to reload transformations.
- Open Power Query Editor to explore applied steps for each sheet.
  &nbsp;
  
**REPOSITORY STRUCTURE**
```
PowerQuery_Project/
│
├── PowerQuery_ETL_Projects.xlsx      ➜    Final Consolidated workbook with all project outputs
│
├── Raw_Files/
│   ├── M01.xlsx                      ➜ Employee Data Raw
│   ├── students and courses.xlsx     ➜ Student and Course Data Raw
│   ├── Consolidation_Files/          ➜ Projects for Consolidation Raw
│   │   ├── Project-alpha.xlsx
│   │   ├── Project-beta.xlsx
│   │   ├── Project-something.xlsx
│   │   ├── Project-something-else.xlsx
│   │   └── Project-new.xlsx
│
├── Screenshots/
│   ├── 1. EmployeeData_AppliedSteps.png
│   ├── 2. WebScraping_Unpivot.png
│   ├── 3. FolderConsolidation_Transform.png
│   ├── 4. StudentCourse_Append_Merge.png
│   └── 5. FemaleStudents_Filter.png
│
└── README.md
```

**_Designed and documented by [Muskan Tayal](https://www.linkedin.com/in/muskan-tayal-820145225)_**
