# Supply-Chain-Data-Analysis-using-AI-Tools-n8n-Quadratic-
This project focuses on building end-to-end analytics solutions using modern AI tools (n8n &amp; Quadratic) within the supply chain domain.

## 🔍 **Project Overview**  

This project focuses on building a **complete data analytics solution** using **modern AI tools – n8n & Quadratic** – within the **supply chain domain**.  

Developed under the mentorship of **Codebasics**, this initiative applies their structured curriculum and data resources to create a robust pipeline: from **email-based data ingestion**, to **PostgreSQL storage**, to **AI-powered data transformation and visualization**.

---

## 🧭 **Project Objectives**  
- ✅ Automate the supply chain data pipeline using **n8n**  
- ✅ Store and organize sales data in a **PostgreSQL** database (hosted on **Supabase**)  
- ✅ Connect and analyze data through **Quadratic**, an AI-powered spreadsheet  
- ✅ Create auxiliary tables like **date dimensions** and **exchange rates** using **AI prompts**  
- ✅ Merge and clean data into a final **fact summary** sheet for analysis  
- ✅ Demonstrate the power of **no-code/low-code AI tools** with a strong foundation in data concepts  

---

## 🛠️ **Tech Stack & Tools Used**  
| Tool | Purpose |
|------|---------|
| 🟢 n8n | Workflow automation, data extraction & transformation |
| 🟣 Supabase | Cloud-hosted PostgreSQL database |
| 📊 Quadratic | AI spreadsheet for querying, cleaning, and analysis |
| 🧠 Python (via AI) | Behind-the-scenes data cleaning, transformation |
| 📩 Gmail | Source of incoming sales data (CSV format) |
| 🔗 OpenExchangeRates.org | Currency conversion API |

---

## 🧩 **Step-by-Step Workflow**

### 1️⃣ **📥 Data Acquisition via Email**  
CSV sales files for **India & USA** were shared via email. Each email contained:  
- Aggregate order data (Order ID, Customer ID, Date)  
- Line item data (Product ID, Quantity, Price)

---

### 2️⃣ **🔄 Automating Ingestion with N8N**  
- Configured Gmail trigger to monitor inbox every minute for new emails with subject “daily sales”  
- Extracted attachments and converted CSVs to **JSON** using n8n nodes  

---

### 3️⃣ **🛢️ Loading into PostgreSQL via Supabase**  
- Parsed and transformed JSON data  
- Converted date formats (e.g., `DDMMYY` ➝ `YYYY-MM-DD`)  
- Inserted data into **two fact tables** and **three dimension tables** hosted on Supabase  

---

### 4️⃣ **🧠 Querying in Quadratic**  
- Established connection to PostgreSQL  
- Pulled fact and dimension tables into separate spreadsheet sheets  

---

### 5️⃣ **📅 Creating Auxiliary Tables using AI Prompts**  
- **Dim Date Table**: Generated using AI Python code based on a custom date range  
- **Exchange Rates Table**: Used OpenExchangeRates API to get USD ➝ INR conversion  

---

### 6️⃣ **🧼 Data Cleaning & Merging (Fact Summary)**  
- AI-generated Python code to:
  - Merge fact and dimension tables  
  - Convert data types, handle missing values  
  - Add **total amount column** (INR-adjusted)  
- Result: A clean, analysis-ready **denormalized summary table**  

---

## 📚 **Key Learnings & Takeaways**

🔸 **AI tools can boost productivity**, but **domain knowledge remains irreplaceable**.  
🔸 A strong grip on **Python, analytics logic, and supply chain concepts** is essential to:  
- Validate AI outputs  
- Spot hallucinations/errors  
- Guide the AI effectively via precise prompts  

---

## 📈 **Final Outcome**  
A fully automated pipeline that:  
- Ingests CSV files from email 📧  
- Transforms and loads data into a cloud database ☁️  
- Uses an AI spreadsheet for querying, cleaning, and analyzing data 🤖  

The project is a perfect blend of **low-code automation** and **high-level analytics thinking**.

---

## 🙌 **Acknowledgments**  
Special thanks to [**Codebasics**](https://codebasics.io) and Dhaval Patel for providing the foundation, inspiration, and learning materials that mad
