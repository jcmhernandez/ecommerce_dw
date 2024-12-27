# E-Commerce & Warehouse Intelligence Platform (EWIP)
Below are summary for each section. Details are available on the pdf file.

## I. Introduction / Background
The E-Commerce & Warehouse Intelligence Platform (EWIP) is a comprehensive data warehouse and analytical solution designed to enhance the performance of analytical data queries. This platform is particularly essential for e-commerce businesses that lack Online Analytical Processing (OLAP) databases and rely on transactional databases for analytics and reporting.

## II. Business Case
EWIP addresses the need for centralized and standardized data storage, and reporting for efficient querying performance. It transforms data from multiple PostgreSQL-based information systems into a dimensional model, enabling better support for historical analysis, business intelligence, and data-driven decision-making.

## III. Business Questions
The platform is designed to answer key business questions related to:
- Platform Performance
- Shop Performance
- Item Performance
- Warehouse Performance
- Warehouse Staff Performance

## IV. Project Timeline
1. **Week 1–2**: Requirement Analysis
2. **Week 3–4**: Data Modeling
3. **Week 5–6**: ETL Implementation
4. **Week 7**: Testing and Validation
5. **Week 8–10**: User Acceptance Test and Revisions
6. **Week 11**: Deployment and Cascade

## V. Proposed System Architecture
### a. High-Level System Architecture
The proposed system integrates data from four PostgreSQL-based information systems into a centralized data warehouse, enabling seamless querying and reporting.

### b. Data Marts
- **Marketplace Data Mart**: Focused on e-commerce transactions and marketplace metrics.
- **Warehouse Data Mart**: Designed for inventory and order fulfillment analytics.

### c. Data Layers
The data warehouse were designed to have various types of tables to support various use cases.
- 20 dimension tables
- 8 detailed fact tables
- 5 summary fact tables
- 3 snapshot fact tables

### d. Data Model
The platform follows a star schema design for simplicity and efficient querying,

### e. ETL Process
The Extract-Transform-Load (ETL) process is designed for efficient data extraction, cleaning, transformation, and loading into the data warehouse. The process for the dim and fact tables were presented in the paper.

### f. Metadata Documentation
Plans for documentation and optional metadata data mart were presented.

## VI. Physical Design of Your Data Engineering Solution
### a. Architectural Overview and Implementation Details
The platform leverages the Google Cloud environment for hosting the data warehouse, alongside tools such as dbt for transformations, Airflow for orchestration, and Power BI for reporting.

### b. SQL Scripts for Implementations
Detailed SQL scripts manage data extraction, transformation, and loading processes, including:
1. Importing libraries.
2. Extracting data from source tables.
3. Comparing new and changed data with the master table.
4. Cleaning data and inserting into error tables.
5. Processing clean data and updating master tables.

### c. Proposed Data Warehouse Design
The data warehouse is optimized for OLAP queries, featuring high scalability and performance.

## VII. Reports Generation
Reports can be generated using tools like Power BI and Google Sheets, providing actionable insights into key business metrics.

## VIII. Project Management
A Gantt chart was presented.

## IX. Conclusion
EWIP provides a competitive advantage through centralized data storage, enhanced analytics capabilities, and seamless reporting. By integrating tools like dbt, Airflow, and Power BI, the platform supports end-to-end data engineering needs, empowering e-commerce businesses with data-driven decision-making.
