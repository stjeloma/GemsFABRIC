# LakehouseBot.ipynb

### Empowering Data Analysis with LangChain-OpenAI and Microsoft Fabric

**Description:**

In the world of modern data analysis, combining cutting-edge language models like OpenAI with the power of Spark SQL and Microsoft Fabric is a game-changer. This article demonstrates how to integrate LangChain-OpenAI into a Microsoft Fabric Notebook with PySpark, leveraging a Lakehouse to store and query data. This setup allows us to turn natural language questions into complex SQL queries seamlessly.

Here’s a quick overview of what we’ll cover:

1. Setting up LangChain-OpenAI with Azure.
2. Leveraging Microsoft Fabric Notebooks with PySpark.
3. Using a Lakehouse for storage and querying of data tables.
4. Converting user questions into SQL queries and running them on Spark.
5. Let’s dive into the details and see how these technologies come together to unlock powerful insights.


# ExploringDeltaTable.ipynb

### Exploring Delta Lake in Microsoft Fabric: A Relational Perspective

**Description:**

Time Travel in Action: Our sales table grew day by day from 2015 to April 2024, reaching 211.9 million records in the latest version. Thanks to Time Travel, we could query the data for any specific day, starting with 23,293 records in version 0 to the full dataset in version 3397. Seamless historical analysis!

Optimized Storage: Using Delta Lake’s OPTIMIZE command, we compacted 3,398 small files into just 3 while keeping the total storage size nearly identical. Faster queries, same efficiency.

Testing Duplicate Appends: We appended the entire dataset twice, pushing the record count to 635 million. Surprisingly, the physical storage size barely increased, proving Delta Lake’s smart handling of identical data.

Unique Key Inserts: In another test, we added 211 million new records with unique OrderKey values but identical columns otherwise. The record count doubled, and while storage size increased due to unique keys, columnar compression minimized the impact.

**Key Takeaway:** 

For those transitioning from SQL Server to Microsoft Fabric, this new architecture powered by Delta Lake and Microsoft OneLake is a solid bet. It combines scalability, efficiency, and flexibility for modern analytics while retaining the reliability you’re used to in the relational world.
_____________________________________

# MonitoringArtifact.ipynb

### Monitoring Artifact runs in Microsoft Fabric

**Description:**

This Python script use the Microsoft Fabric API ready-to-use to fetch and display the latest runs details of any artifact.

*UPDATE 12-19-2024*: Today with new version of [semantic-link-labs 0.8.11](https://github.com/microsoft/semantic-link-labs/releases/tag/0.8.11) (thanks **Michael Kowalsky**)
_____________________________________

# Automated Tables Shortcuts.ipynb

### Automating Table Shortcuts in Microsoft Fabric for Unified Data Strategy in OneLake

**Description:**

This Notebook script demonstrates how to automate the creation of shortcuts for tables between a source Workspace and Lakehouse and a destination Workspace and Lakehouse in Microsoft Fabric. This approach supports the "single source of truth" strategy in OneLake and aligns with the Medallion architecture by simplifying data access and management across workspaces. The script uses Microsoft Fabric APIs to list tables in the source Lakehouse and creates corresponding shortcuts in the destination Lakehouse.

**Key Benefits:**
- Centralized Data Access: This code aligns with the "single source of truth" strategy by enabling access to tables in different Lakehouses without duplicating data.
- Simplified Management: Reduces operational overhead by automating shortcut creation.
- Medallion Architecture Support: Facilitates the creation of Bronze, Silver, and Gold layers in Microsoft Fabric through seamless data linking.

I want to express my gratitude to Michael Kovalsky https://www.linkedin.com/in/michaelkovalsky/ for all the outstanding work on the semantic-link-labs library, and to Sandeep Pawar https://www.linkedin.com/in/sanpawar/ for being a constant source of inspiration with every one of his posts.
