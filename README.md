# Automating Table Shortcuts in Microsoft Fabric for Unified Data Strategy in OneLake

**Description:**

This Notebook script demonstrates how to automate the creation of shortcuts for tables between a source Workspace and Lakehouse and a destination Workspace and Lakehouse in Microsoft Fabric. This approach supports the "single source of truth" strategy in OneLake and aligns with the Medallion architecture by simplifying data access and management across workspaces. The script uses Microsoft Fabric APIs to list tables in the source Lakehouse and creates corresponding shortcuts in the destination Lakehouse.

**Key Benefits:**
- Centralized Data Access: This code aligns with the "single source of truth" strategy by enabling access to tables in different Lakehouses without duplicating data.
- Simplified Management: Reduces operational overhead by automating shortcut creation.
- Medallion Architecture Support: Facilitates the creation of Bronze, Silver, and Gold layers in Microsoft Fabric through seamless data linking.

I want to express my gratitude to Michael Kovalsky https://www.linkedin.com/in/michaelkovalsky/ for all the outstanding work on the semantic-link-labs library, and to Sandeep Pawar https://www.linkedin.com/in/sanpawar/ for being a constant source of inspiration with every one of his posts.
