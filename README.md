# 🏥 Healthcare Management System: SQL Analytics Portfolio

## 📄 Project Overview
This project demonstrates the design and implementation of a comprehensive **Relational Database Management System (RDBMS)** for a healthcare environment. As a Data Analyst, I focused on creating a scalable schema and writing complex SQL queries to extract meaningful insights regarding hospital operations, patient demographics, and resource allocation.

The project transitions from **Database Design (DDL)** to **Data Manipulation (DML)** and culminates in **Advanced Business Intelligence (BI) Queries**.

---

## 🛠️ Technical Stack
* **Language:** SQL (MySQL)
* **Key Concepts:** Relational Schema Design, Data Normalization, Joins, CTEs (Common Table Expressions), Window Functions, and Aggregate Analysis.

---

## 📊 Database Architecture
The database consists of **8 interconnected tables** designed to maintain high data integrity:
* `hospitals` & `departments`: Organizational hierarchy.
* `doctors` & `patients`: Professional and demographic data.
* `appointments`, `prescriptions`, `rooms`, & `medications`: Transactional and operational records.

---

## 💡 Key Analytical Insights
The following business questions were solved using advanced SQL techniques:

### 1. Operational Efficiency & Ranking
* **Medication Trends:** Identified the **3rd most frequently prescribed medication** using `LIMIT` and `OFFSET` to assist in pharmaceutical inventory planning.
* **Capacity Audits:** Used `DENSE_RANK()` over partitions to identify the department with the **second-largest room capacity** within each specific hospital.
* **Staffing Levels:** Leveraged **CTEs (Common Table Expressions)** to isolate hospitals currently operating with the lowest doctor-to-hospital ratio.

### 2. Patient Demographics & Emergency Management
* **Segmented Analysis:** Categorized emergency patients into **Pediatric, Adult, and Geriatric** groups using `CASE` statements to better understand age-related facility requirements.
* **Engagement Metrics:** Filtered high-frequency patients (those with >3 appointments) to identify chronic care needs using `HAVING` and `GROUP BY`.

### 3. Data Integrity & Cleaning
* **Missing Records Audit:** Used `LEFT JOIN` to identify patients who were seen by doctors but did not receive a prescription, ensuring clinical compliance.
* **Age Calculation:** Utilized `TIMESTAMPDIFF` to dynamically calculate patient ages from `DOB` for real-time reporting.

---

## 🚀 How to Run
1. Clone this repository.
2. Open the `sql_project.sql` file in your preferred SQL editor (MySQL Workbench, DBeaver, etc.).
3. Execute **PART 1** to initialize the `hospital_system` database and populate the records.
4. Execute **PART 2** to run the analytical queries and view the results.

---


**GitHub:** [github.com/duaajaved321](https://github.com/duaajaved321)
