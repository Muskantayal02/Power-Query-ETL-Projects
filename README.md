_Designed and documented by [Muskan Tayal](https://www.linkedin.com/in/muskan-tayal-820145225)_

**PROJECT OVERVIEW:**

This repository showcases multiple **ETL (Extract, Transform, Load)** projects built using **Power Query**. Each project demonstrates how real-world data challenges - from messy Excel sheets to combining datasets across files - can be solved through systematic data cleaning, transformation, and automation techniques.

All project outputs are consolidated in one Excel workbook:
**`PowerQuery_ETL_Projects.xlsx`**

Each sheet within this workbook represents a standalone project demonstrating a specific Power Query functionality.

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

**PROJECT SUMMARIES**

**A) Employee Data Cleanup:** (_Sheet Name - Employee Data Cleaning_)

**Goal:** Clean and prepare HR dataset for reporting.

**Steps:**
* Removed blank rows and unnecessary columns
* Promoted headers and replaced null values
* Extracted country names from location column using “Column from Examples”
* Standardized departments and filtered out ex-employees
* Transformed data types (date, currency, text)

![Applied Steps – Employee Data](1.EmployeeData_AppliedSteps.png)

**Outcome:** A clean employee dataset ready for payroll and demographic reporting.

**Skills:** Data cleaning, type transformation, text extraction.


**B) Web Scraping - India Population Data**  (_Sheet Name - India Population Web_)

**Goal:** Transform a messy web dataset into a structured table.

**Steps:**
* Imported HTML table directly from a government site
* Removed extra rows and columns, promoted headers
* Unpivoted year columns to normalize the data
* Extracted year numbers from text and cleaned population column
* Removed null/error rows and standardized column types

**Outcome:** A long-format dataset for population trends by state and year.

**Skills:** Web data extraction, unpivoting, string parsing, data validation.


**C) Excel Files Consolidation**  (_Sheet Name - Projects Consolidation_)

**Goal:** Combine monthly project data from multiple Excel files into one master table.

**Steps:**
* Imported all `.xlsx` files from a folder using *From Folder* connector
* Transformed sample file, standardized project names (removed `.xlsx`)
* Added a custom column to convert month numbers into date values
* Filtered to include only Excel files, changed types, and loaded final dataset
* Tested automation by adding a new file and refreshing queries successfully

**Outcome:** An automated consolidated project database that refreshes on new file addition.

**Skills:** Folder automation, dynamic ETL, custom column formulas, refresh testing.


**D) Students & Courses (Append and Merge)**  (_Sheet Name - Female Students_)

**Goal:** Combine data from multiple classes and enrich it with course-level details.

**Steps:**
* Imported Class 11 and 12 sheets and added custom “Year” columns
* Appended both tables to create a single student dataset
* Merged the combined dataset with the Course table (teacher, credits, assessment type)

**Outcome:** Unified student-course dataset ready for analytics and academic reporting.

**Skills:** Append queries, merge queries, relational data integration.


**E) Filtering Female Students on ≥3 Courses** (_Sheet Name - Female Students_)

**Goal:** Identify and analyze high-performing female students across multiple courses.

**Steps:**
* Created a reference query from the unified student dataset
* Filtered Gender = Female
* Applied filter for Credits ≥ 3
* Customized load behavior (set support tables as connection-only)

**Outcome:** A filtered, query-based insight table highlighting targeted academic groups.

**Skills:** Query referencing, load optimization, conditional filtering.

**DELIVERABLES**

* **Excel Workbook:** `PowerQuery_ETL_Projects.xlsx` (contains all project sheets) 
* **Raw Files Folder:** Source files for reproducibility
* **Screenshots Folder:** Key snapshots showing Power Query Applied Steps and final outputs

**KEY HIGHLIGHTS**

- Combined **5 distinct Power Query projects** demonstrating versatile ETL capabilities
- Used **Append**, **Merge**, **Unpivot**, **Custom Columns**, **Replace Values**, and **Connection-only Queries**
- Optimized query groups and loading behavior for performance
- Demonstrated both **one-time cleaning* and *refresh-based automation** workflows
- Showcases proficiency across **data preparation, transformation, and integration**

**TECH STACK**

| Tool                               | Purpose                                         |
| ---------------------------------- | ----------------------------------------------- |
| **Microsoft Excel (Power Query)**  | Data extraction, transformation, and automation |
| **GitHub**                         | Documentation and version control               |

**OUTCOME**

- This project demonstrates real-world data handling proficiency using Power Query - from cleaning and merging messy datasets to automating reporting pipelines.
- It reflects hands-on ability to transform raw data into structured, analysis-ready outputs efficiently.

**FUTURE ENHANCEMENTS**

* Link outputs to Power BI dashboards for visualization.
* Integrate data refresh automation with OneDrive or Power Automate.
* Add error-handling and dynamic parameterization for folders and URLs.

**REPOSITORY STRUCTURE**
```
PowerQuery_Project/
│
├── PowerQuery_ETL_Projects.xlsx         Final Consolidated workbook with all project outputs
│
├── Raw_Files/
│   ├── M01.xlsx Employee_Data_Raw
│   ├── students and courses.xlsx
│   ├── Consolidation_Files/
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
