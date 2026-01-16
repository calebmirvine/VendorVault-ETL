# Vendor Procurement Automation Utility

**An automated ETL (Extract, Transform, Load) pipeline designed to modernize supply chain monitoring.**

This utility bridges the gap between external vendor APIs and internal business intelligence tools. By automating the retrieval of real-time pricing and inventory data, it eliminates manual data entry, allowing procurement teams to focus on analysis rather than collection.

## 📉 Business Impact & Value

* **90% Reduction in Overhead:** Reduced daily administrative checks from hours to minutes.
* **Scalability:**Capable of auditing hundreds of SKUs simultaneously without additional labor.
* **Cost Avoidance:** Identifies price fluctuations and stock volatility in real-time, preventing purchasing errors and overpayment.

## 🔄 Logistics & Workflow Utilization

This script acts as the data engine for a larger automated ecosystem:

1.  **Extraction (Python):** Script authenticates via OAuth2 and pulls live data from the vendor's API based on a target CSV list.
2.  **Automation (Power Automate):** The generated report is detected by Microsoft Power Automate Desktop.
3.  **Integration (SharePoint):** Data is parsed and appended to a master Excel dataset on SharePoint.
4.  **Analysis (Excel):** Procurement managers utilize **Pivot Tables** connected to this master data to visualize trends and forecast inventory needs.

## 🛠️ Technical Stack

* **Language:** Python 3.10+
* **Libraries:** `pandas` (Data aggregation), `requests` (Authenticated API calls), `python-dotenv` (Security).
* **Security:** Credentials managed via environment variables; endpoints obfuscated for privacy.

## ⚙️ Quick Setup

1.  **Install Dependencies:** `pip install pandas requests python-dotenv`
2.  **Configure Env:** Create `.env` with `VENDOR_API_TOKEN`, `USERNAME`, and `PASSWORD`.
3.  **Load Data:** Place target URLs in `./data/input_product_list.csv`.
4.  **Run:** Execute `python3 main.py` to generate the report.

> **Note:** Specific vendor endpoints and credentials in this repository have been obfuscated.
