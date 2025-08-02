# Placement-Eligibiity-Application

**Project Description**
- An interactive Student Placement Eligibility dashboard to fetch student's placement eligibility details based on the filters applied.
- This web application developed using Python , MySQL and Streamlit.
- It helps colleges or placement coordinators to evaluate which students are ready for placement based on various metrics such as technical, and soft skill.

**Project Overview**

By connecting to a structured student database, the app allows users to apply filters such as:
- Minimum soft skills average score,
- Number of problems solved,
- Assessments completed,
- Mini projects,
- Mock interview scores,
- Placement status.

It displays only those students who meet the eligibility criteria.
Additionally, the dashboard provides predefined insights from the database using custom SQL queries, including:
- Top students with strong critical thinking or communication skills,
- Batch-wise average performance,
- Placement trends over graduation years,
- Top students by package,
- Students who earned certifications and got placed.

The application makes it easier for decision-makers to identify high-performing students, monitor readiness levels, and track placement outcomes effectively.

## 🛠️ Technologies Used

| Component     |                Description                         |
|---------------|----------------------------------------------------|
| **Python**    | Core programming language                          |
| **Streamlit** | Web app framework for dashboard UI                 |
| **MySQL**     | Backend relational database                        |
| **pandas**    | For data manipulation and reading SQL queries      |
| **SQL**       | For extracting insights and filtering student data |


## 🔄 Project Flow

### 1. **Database Connection**
- The app connects to a local MySQL database using `mysql.connector`.
- Tables used: `students`, `programming`, `soft_skills`, `placements`.

### 2. **Filter Section (Sidebar)**
- Users can apply filters such as:
  - Minimum average soft skills score
  - Problems solved
  - Assessments completed
  - Mini projects
  - Mock interview score
  - Placement status (Placed / Ready / Not Ready / All)

### 3. **Eligible Students Table**
- Based on the selected filters, the app runs a dynamic SQL query.
- Shows the list of students who meet the selected criteria using `pandas.read_sql()` and displays it in a table.

### 4. **Placement Insights Section**
- Dropdown with 10 insightful SQL-based queries like:
  - Average programming performance per batch
  - Top 5 students ready for placement
  - Students with good critical thinking
  - Top communicators
  - Graduation year-wise placement count
  - Top placed students by package
  - Certification holders who got placed
 
  

Creator - Yuvaraj Vijayaraj






