# Data Warehouses Business Analysis Project

## What the Project Does
This project focuses on building and analyzing data warehouses to support business intelligence and decision-making processes. It includes scripts, schemas, and data for creating and managing a data warehouse, as well as tools for analyzing and visualizing the data.

## Why the Project is Useful
- **Centralized Data Management**: Consolidates data from multiple sources into a single repository.
- **Business Insights**: Enables efficient querying and reporting for business analysis.
- **Scalable Architecture**: Provides a foundation for scaling data operations as business needs grow.

## How Users Can Get Started

### Prerequisites
- **Database Management System**: PostgreSQL or any compatible database.
- **Python Environment**: Python 3.10+ with required dependencies.
- **Tools**: SQL client (e.g., pgAdmin, DBeaver) for database interaction.

### Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Data_Warehouses_Business_Analysis_Project
   ```
2. Install Python dependencies:
   ```bash
   pip install -r reqs/requirements.txt
   ```
3. Unzip the data files:
   ```bash
   unzip Data/data_berka.zip -d Data/
   unzip DataWarehouse/bank_dw_neon.zip -d DataWarehouse/
   ```
4. Set up the database:
   - Use the SQL scripts in the `Schemas/` directory to create the source, staging, and data warehouse schemas.
   - Example:
     ```bash
     psql -U <username> -d <database> -f Schemas/source_schema_sql.sql
     ```

### Usage
- Load data into the source schema using the provided scripts.
- Transform and stage the data using the staging schema.
- Query the data warehouse schema for business insights.

## Where Users Can Get Help
- **Documentation**: Refer to the SQL scripts and comments in the codebase.
- **Issues**: Report bugs or request features via the GitHub Issues tab.
- **Community**: Join relevant forums or communities for data warehousing and business analysis.

## Who Maintains and Contributes
- **Maintainer**: Mihai (mihae)
- **Contributions**: Contributions are welcome! Please follow the guidelines in `CONTRIBUTING.md` (if available).

---

Feel free to reach out for support or collaboration opportunities!
