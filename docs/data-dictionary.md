# 📋 Data Dictionary — Sample Hiring Dataset

---

## 📄 Sheet: Applicant_Data

| Column Name | Data Type | Description | Example |
|-------------|-----------|-------------|---------|
| Applicant_ID | Text | Unique identifier for each applicant | APP-001 |
| Job_ID | Text | ID of the role applied for | JOB-2024-05 |
| Department | Text | Department the role belongs to | Talent Acquisition |
| Source | Text | Channel through which applicant was sourced | LinkedIn, Referral, Job Board |
| Application_Date | Date | Date the application was submitted | 01-Jan-2024 |
| Stage | Text | Current stage in the hiring funnel | Screened / Interviewed / Offered / Hired / Rejected |
| Offer_Extended | Boolean | Whether an offer was made | Yes / No |
| Offer_Accepted | Boolean | Whether the offer was accepted | Yes / No |
| Offer_Date | Date | Date offer was extended | 20-Jan-2024 |
| Acceptance_Date | Date | Date offer was accepted | 22-Jan-2024 |

---

## 📄 Sheet: Hire_Data

| Column Name | Data Type | Description | Example |
|-------------|-----------|-------------|---------|
| Hire_ID | Text | Unique identifier for each hire | HIRE-001 |
| Applicant_ID | Text | Links back to Applicant_Data | APP-001 |
| Job_ID | Text | Role that was filled | JOB-2024-05 |
| Hire_Date | Date | First day on the job | 01-Feb-2024 |
| Source | Text | Sourcing channel | LinkedIn |
| Time_to_Hire_Days | Number | Days from job open to offer acceptance | 28 |

---

## 📄 Sheet: Post_Hire_Performance

| Column Name | Data Type | Description | Example |
|-------------|-----------|-------------|---------|
| Hire_ID | Text | Links back to Hire_Data | HIRE-001 |
| Retained_at_90_Days | Boolean | Still employed at 90 days | Yes / No |
| Manager_Score_90D | Number (1–5) | Manager satisfaction at 90 days | 4 |
| Performance_Rating | Number (1–5) | Performance score at first review | 3.5 |
| Quality_of_Hire_Score | Number (0–100) | Composite score (auto-calculated) | 76 |

---

## 📄 Sheet: Cost_Data

| Column Name | Data Type | Description | Example |
|-------------|-----------|-------------|---------|
| Job_ID | Text | Role reference | JOB-2024-05 |
| Recruitment_Cost | Currency | Ad spend + agency fees + interviewer hours | ₹45,000 |
| Onboarding_Cost | Currency | Training + equipment + admin | ₹20,000 |
| Productivity_Loss_Cost | Currency | Estimated cost of reduced output during ramp-up | ₹60,000 |
| Bad_Hire_Flag | Boolean | Was this identified as a bad hire? | Yes / No |
| Total_Bad_Hire_Cost | Currency | Total cost if flagged as bad hire | — |

---

*Note: All data is sample/synthetic data created for learning purposes only.*
