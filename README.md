<div align="center">
	<img src="https://github.com/user-attachments/assets/82c7ae69-c772-4610-a898-14d63007f2f9">
</div>

<h1 align="center">
Deshpande Foundation Projects
</h1>

<div align="center">
    <strong> All the project descriptions that are done in the Deshpande Foundation</strong>
</div>


# Project 1: LEAD Data Analysis

**Dashboard:** *[Dashboard Link](https://analytics.zoho.in/open-view/286995000004644969)*

## Dashboard Requirements

- ### Overview Dashboard:
   * Total project and student count.
   * Project status breakdown (Proposed, In Progress, Completed).
- ### Trainer Performance Report:
   * Trainer-wise project status distribution.
   * Training sessions conducted and student feedback.
- ### Student Progress Report:
   * Student-wise project status and progress.
   * Participation metrics (number of projects, impact).
- ### Manager Performance Report:
   * Manager-wise project funding allocation.
   * Project distribution by manager.
- ### Regional Analysis:
   * District-wise project and student participation.
   * Fund distribution across districts.
- ### Dashboard Features:
   * Interactive filters and drill-down options.
   * Data export and custom alerts.
 
## Problem Analysis
- **Duplicate Data Issue:** Excessive duplication in the dataset, which needs to be resolved for accurate analysis.
  
- **Disproportionate Manager Data:** The Manager table has around 140 unique manager IDs but contains 173,000 rows, indicating data redundancy or repeated entries.
  
- **Dashboard and MIS Report Mismatch:** There's a discrepancy in the data count between the dashboard and the Management Information System (MIS) report. 

## Solution
- **Duplicate Data Removal:** After discussing with Sharad, the duplicate data was removed, allowing for accurate report and dashboard creation.

- **Data Mismatch Investigation:** To understand the data mismatch, the backend of the MIS dashboard needs to be checked, particularly the date ranges used.
  
- **Feature Differences:** There are some differences in features between the MIS and Zoho systems, making a 100% data match impossible. 


# Project 2: SiV Data Analysis

## Dashboard Requirements
- ### Institute-Wise Attendance Report:
    * Display attendance percentages for each institute.
    * Identify trends in attendance over time.
- ### KLE Colleges Attendance:
    * Show attendance percentage specifically for KLE colleges.
    * Compare KLE college attendance to other institutes.
- ### Student-Wise Payment Report:
    * Track payments made by each student, including outstanding balances.
    * Display payment history and recent payment dates.
- ### Institute-Wise Schedule Update Report:
    * Provide updates on schedule changes for each institute.
    * Include information on upcoming events or sessions.
- ### Dashboard Features:
    * **Interactive Filters:** Filter by institute, date range, or student.
    * **Drill-Down Options:** Click for detailed data on individual students or institutes.
    * **Automated Alerts:** Notifications for overdue payments or attendance below a set threshold.
    * **Data Export:** Download reports for further analysis or sharing.

## Problem Analysis
- **Duplicate Attendance Tables:** There were two attendance tables containing the same data, causing redundancy.
  
- **Missing Schedule Table:** The schedule table was absent, impacting the ability to track and update schedules.
  
- **Duplicate Student Data in Admission Table** The student admission table contained duplicate records, leading to inconsistencies.
  
- **High Data Volume Impact:** The attendance table had 4.4 million records, causing the database to go into standby mode when Zoho attempted to fetch data, due to capacity limitations.


## Solution
- **Duplicate Data Removal:** After discussing with Anand, the duplicates in the student admission table were removed, and he confirmed which attendance table should be used.
  
- **Schedule Data Update:** Anand mentioned he would add the schedule data, but it has not yet been reflected in the database.
  
- **Data Overload Issue:** After consulting with Sharad, all live connections for SiV in Zoho were deleted, resulting in the removal of all reports. The only suggested solution to handle the data load was to increase the server capacity.


<h2 align="center">Now the Project is on hold until further notice.</h2>


# Project 3: Skillplus Placement Data Analysis

**Dashboard:** *[Dashboard Link](https://analytics.zoho.in/open-view/286995000005063717)*


## Dashboard Requirements
- ### Year-Wise Placement Status Report:
    * Display the count of placements for each year.
    * Track trends in placement rates over time.
- ### Program-Wise Placement Status Report:
    * Show placement counts for different programs (e.g., S3, S4).
    * Compare placement success rates across programs.
- ### Student-Wise Company Count:
    * Track the number of companies each student has been placed in or received offers from.
- ### Company-Wise Student Count:
    * Display the number of students placed in each company.
    * Highlight companies with the highest placement intake.
- ### Average CTC (Cost to Company):
    * Calculate and display the average CTC offered to placed students.
    * Compare average CTC across different programs and years.
- ### Dashboard Features:
   * **Interactive Filters:** Filter data by year, program, company, or student.
   * **Drill-Down Options:** View detailed information on specific students or companies.
   * **Automated Alerts:** Notifications for significant changes in placement trends or CTC.
   * **Data Export:** Download placement reports for further analysis or sharing.
 
## Problem Analysis
- **Multiple Placement Data Tables:** There are several tables containing placement data, leading to potential inconsistencies and confusion in data management.
  
- **Missing Student Status:** None of the tables include the student status, which is essential for tracking placement outcomes.
  
- **Data Limitation by Academic Year:** Only data from the Academic Year 2023–2024 is available, as previous years do not include student status information.
  
- **Inconsistent Salary Data:** The Salary column contains non-standardized formats (e.g., '2 LPA - 3 LPA', '200000 - 300000', '20732 per month'), making it impossible to calculate an average CTC accurately.
  
- **Discrepancies in S3 and S4 Student Counts:** The student counts for S3 and S4 do not align with the figures maintained by the Placement Team.

- **Mismatch with Excel Data:** There are inconsistencies between the numbers in the dashboard and the Excel sheet maintained by trainers, as updates occur in both systems without synchronization.

## Solution 
- **Student Status Addition:** Anand added the student status to a table, but it currently only includes data for the Academic Year 2023-2024.
  
- **Placement Type Update:** Anand also included the Placement Type in the table as requested by the team.
  
- **Salary Data Standardization:** The salary data format issues remain unresolved, preventing accurate calculation of average CTC.
  
- **Data Synchronization:** To ensure consistent numbers, all updates must be made in a single location (i.e., the MIS). If existing data mismatches are corrected in the MIS, the dashboard will reflect accurate information.
  
- **Reporting:** A detailed report was provided to both the Placement Team and the Tech Team in two separate Google Sheets, with links shared for reference.
Dashboard Submission: The updated dashboard was submitted to the team for their review.


# Project 4: Skillplus EZY Attendance Data Analysis

**Dashboard:** *[Dashboard Link](https://analytics.zoho.in/open-view/286995000004503378)*

## Dashboard Requirements
- ### Daily Report:
    * **Actual Cohort Count:** Total participants.
    * **Engaged Cohort Count:** Actively engaged participants.
    * **Not Engaged Count:** Participants not engaged.
    * **Total Sessions:** Overall sessions conducted.
    * **Attendance Breakdown:** Counts for >95%, 91%-94%, 85%-90%, 81%-84%, and <80%.
    * **Duration Breakdown:** Counts for >120 min, 90-120 min, 60-90 min, and <60 min.
- ### Periodic Report:
    * **Number of Working Days:** Total working days.
    * **Engaged Cohort Count:** Engaged participants.
    * **Not Engaged Count:** Non-engaged participants.
    * **Total Sessions Count:** Sessions conducted.
- ### Dashboard Features:
    * **Interactive Filters:** Filter by date or cohort.
    * **Drill-Down Options:** Access detailed info.
    * **Automated Alerts:** Notify for engagement changes.
    * **Data Export:** Download reports for analysis.

## Problem Analysis
- **Closed Cohorts in Admission Table:** The admission table includes cohort names that have already been closed, complicating the total cohort count.
  
- **Data Filtering Issues:** When applying filters, the actual cohort count is also affected, leading to negative values for the not engaged count (calculated as Actual cohort - Engaged cohort).

- **Database Performance:** The large volume of data occasionally causes the database to go into standby mode when loading the dashboard, impacting performance and accessibility.

## Solution
- **Cohort Table Request:** I requested Sharad to create a separate table containing all cohort names, their status, and the associated programs. This will stabilize the actual cohort count even when using date filters.

- **Problem Resolution:** After discussions with Sharad, the issue was addressed; however, displaying the not engaged cohort count was concluded to be unfeasible without the cohort table.

- **Dashboard Submission:** The dashboard was completed and submitted to the team without the cohort table.

- **Summarized Attendance Table:** I asked Sharad about the possibility of creating a summarized attendance table and provided him with a sample format that includes the required columns. This approach aims to reduce the database load and prevent it from going into standby mode.


# Project 5: Skillplus Academics Data Analysis

**Dashboard:** *[Dashboard Link](https://analytics.zoho.in/open-view/286995000000490372)*

## Dashboard Requirements
- ### Division-Wise Actual Cohort Count:
   * **Program Counts:** Display actual cohort counts for each program (S3, S4) by division.
   * **Active Cohorts:** Count of active cohorts for each program within each division.
   * **Not Active Cohorts:** Count of cohorts that are not active for each program.
- ### Targeted and Actual Business Performance (BP):
   * **Targeted BP:** Display targeted business performance for active cohorts in each program.
   * **Actual BP Covered:** Show the actual business performance covered by the active cohorts.
- ### Dashboard Features:
   * **Interactive Filters:** Filter by division, program, or cohort status.
   * **Data Visualization:** Use charts or graphs to represent active and not active cohorts.
   * **Automated Alerts:** Notifications for any discrepancies between targeted and actual BP.
   * **Data Export:** Download reports for further analysis.
 
## Problem Analysis
- **Lack of Actual Cohort Count:** The current data does not provide the actual count of cohorts in each division, making it impossible to accurately report on the division-wise cohort statistics.

## Solution
- **Cohort Table Acquisition:** Once the cohort table is obtained, it will resolve the issue of missing actual cohort counts in each division.

- **Problem Resolution:** After discussions with Sharad, the issue was addressed.

- **Dashboard Submission:** The dashboard was completed and submitted to the team, despite the absence of the cohort table.


# Project 6: Farm Pond Application Project

## Project Requirements
- ### Project Takeover:
   * Assume full responsibility for the Farm Pond project from the Tech Team.
- ### Technical Understanding:
   * Gain a comprehensive understanding of the database structure, stored procedures, and APIs used in the project.
- ### Documentation:
   * Create detailed documentation for the entire system, including:
   * Database schema and relationships
   * Web application functionality and features
   * Android application functionality and features
- ### Feature Modifications:
   * Identify and implement changes to specific features of the application as needed for improvement or user feedback.
- ### Project Features:
   * **Collaborative Review:** Work with the Tech Team for a smooth transition.
   * **Version Control:** Utilize version control for documentation and code changes.
   * **Testing and Validation:** Ensure thorough testing of any changes made to the application features.

## Problem Analysis
- **Lack of Documentation:** The project currently lacks comprehensive documentation, making it difficult to understand the overall system architecture and functionalities.

- **Absence of Data Flow Diagram:** There is no clear data flow diagram, which hinders the understanding of how data moves through the system.

- **Undefined Application Workflow:** The application workflow is not properly documented, leading to potential confusion about user interactions and processes within the application.

## Solution
- **Application Workflow Documentation:** Developed comprehensive documentation outlining the application workflow, detailing user interactions and processes.

- **Database Documentation:** Created detailed documentation of the database, including schema, relationships, and data types.

- **System Architecture:** Established a clear system architecture diagram to visualize the overall structure and components of the project.

- **API and Stored Procedure Documentation:** Documented all APIs and stored procedures, providing descriptions of their functionality and usage.


# Project 6.1: Help GIS Team

## Project Requirements
- ### GIS Team Collaboration:
    * Engage with the GIS team to fully understand their requirements and objectives.
- ### Data Processing with QGIS:
    * Utilize QGIS to clip Land Use Land Cover (LULC) and soil data based on specified watershed boundaries.
- ### Rainfall Data Analysis:
    * **Assist the GIS team in summarizing hourly rainfall data into:**
      * Monthly averages and sums
      * Yearly averages and sums
      * Implement this data processing using Python for efficiency and accuracy.
- ### Project Features:
    * **Interactive Meetings:** Regular discussions with the GIS team to ensure alignment on goals.
    * **QGIS Tools:** Leverage appropriate QGIS tools for effective data clipping and visualization.
    * **Python Scripts:** Develop reusable Python scripts to automate the summarization of rainfall data.


