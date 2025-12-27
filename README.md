# 📊 Ticket Management Reporting Automation – L2 Support

## 🧩 Project Overview
This project implements an **end-to-end automation** for generating and distributing **ticket management reports for a Level 2 (L2) Support team**.

The workflow consolidates data from Atlassian tools (simulated through a **Mock API**), processes key operational metrics, and distributes **periodic reports to stakeholders**, enabling visibility into ticket volume, trends, and main demand drivers.

---

## 🎯 Objective
Automate and standardize the reporting process by:
- Automatically consolidating resolved tickets
- Processing operational support metrics
- Providing visibility into ticket volume by **Category** and **Request Type**
- Identifying **top offenders** (categories and request types with the highest incoming volume)

---

## ⚙️ Technologies & Tools
- **n8n** – Workflow automation (low-code)
- **Jira (simulated via Mock API)** – Ticket source
- **JSON** – Data structure
- **Google Sheets (online)** – Data persistence
- **Email (SMTP)** – Report distribution
- **GitHub** – Version control and documentation

---

## 🔄 Workflow Process

1. **Ticket retrieval**
   - Tickets are queried from Jira  
   - For demonstration purposes, a **Mock API** is used to simulate real ticket data

2. **Time-based filtering**
   - Selection of **resolved tickets** within a defined time period

3. **Data cleaning & normalization**
   - Removal of unnecessary fields
   - Normalization of categories and request types

4. **Metrics processing**
   - Aggregation by:
     - Category
     - Request Type
   - Calculation of resolved ticket volume

5. **Data persistence**
   - Processed data is stored in an **online Google Sheet**

6. **Distribution**
   - Automatic **email delivery with embedded tables**
   - Reports include:
     - Ticket volume by category
     - Ticket volume by request type
     - Top offenders (highest incoming volume)

---

## 📈 Generated Metrics
- Total resolved tickets per period
- Ticket volume by **Category**
- Ticket volume by **Request Type**
- Ranking of highest-demand categories
- Ranking of highest-demand request types

---

## 🧪 Test Data
To avoid using sensitive or real production data:
- Tickets are retrieved from a **Mock API**
- All data is fictional
- The data structure mirrors real-world Jira / ITSM scenarios

---

## 🖼️ Artifacts & Evidence
- Exported n8n workflow (`.json`)
- Workflow screenshots
- Example of generated Google Sheet
- Example of email sent to stakeholders

---

## 🚀 Project Impact
- Reduced manual reporting effort
- Improved operational visibility for the L2 Support team
- Consistent and reusable data for decision-making
- Scalable solution adaptable to production environments

---

## 🔮 Future Improvements
- Include unresolved tickets and SLA tracking
- Add resolution time metrics
- Automated dashboards (Looker / Power BI)
- Scheduled execution (cron-based)
- Direct integration with production Jira

---

## 👩‍💻 Author
**Ana M**  
Automation · Functional Support · Data Analysis · Low-code
