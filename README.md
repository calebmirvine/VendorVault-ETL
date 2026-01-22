Supply Chain & Procurement Automation Tool

**A high-performance asynchronous ETL suite engineered to modernize vendor data retrieval and drive data-backed procurement decisions.**

---

## Business Impact

In typical procurement workflows, maintaining accurate pricing for hundreds of SKUs is a labor-intensive manual process. This solution transforms that friction into efficiency:

* **98% Time Reduction:** Automated data collection reduced processing time from hours of manual entry to **under 60 seconds**.
* **Cost Optimization:** Real-time tracking of price fluctuations across volatile SKUs enables proactive budget management and prevents overpayment.
* **Strategic BI:** Feeds a master analysis suite where **Pivot Tables** and **Historical Trends** empower leadership with actionable quarterly insights.

---

### Core Stack
* **Asynchronous Processing:** Built with `httpx` and `asyncio` to handle multiple API request.
* **Data Engineering:** Leverages `pandas` for advanced deduplication, path management, and structured CSV serialization.
* **Security & Portability:** Environment-driven configuration (`python-dotenv`) ensures total anonymization of proprietary endpoints, while cross-platform binary builds (PyInstaller) enable deployment on Windows, macOS, and Linux.
