**Pipeline Flow**

1. Data stored in Azure Data Lake
        ↓
2. Pipeline (ecomm) moves data
        ↓
3. Data stored in Lakehouse (Bronze)
        ↓
4. Notebook transforms data (Silver → Gold)
        ↓
5. SQL Endpoint enables querying
        ↓
6. Semantic Model (gold_360) used for reporting


<img width="401" height="299" alt="image" src="https://github.com/user-attachments/assets/50517652-c2ae-44e8-90a0-8778c63b4d2a" />
