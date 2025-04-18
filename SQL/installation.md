# SQL Installation Guide

## Required Software

- **Database Management System**: Choose one or more:
  - **MySQL/MariaDB**: Open-source relational database
  - **PostgreSQL**: Advanced open-source database
  - **SQLite**: Lightweight file-based database
  - **Microsoft SQL Server**: Commercial SQL database
  - **Oracle Database**: Enterprise database system
- **Database Client**: For connecting to and querying databases
  - **MySQL Workbench**: GUI for MySQL
  - **pgAdmin**: GUI for PostgreSQL
  - **DBeaver**: Universal database tool
  - **Azure Data Studio**: Cross-platform database tool
- **Command Line Tools**: Database-specific CLI clients

## File Extensions

- `.sql` - SQL script files
- `.db`, `.sqlite`, `.sqlite3` - SQLite database files
- `.mdf`, `.ldf` - SQL Server database files
- `.mwb` - MySQL Workbench model files
- `.dbml` - Database markup language files
- `.ddl` - Data definition language scripts
- `.dml` - Data manipulation language scripts
- `.bak` - Database backup files
- `.dump` - Database dump files
- `.csv`, `.tsv` - Data import/export formats
- `.json` - JSON data import/export format
- `.erd` - Entity relationship diagram files

## Package Management

```bash
# SQL doesn't have traditional package managers
# But you can install database systems:

# Install MySQL (Ubuntu/Debian)
sudo apt update
sudo apt install mysql-server

# Install PostgreSQL (Ubuntu/Debian)
sudo apt update
sudo apt install postgresql postgresql-contrib

# Install SQLite (Ubuntu/Debian)
sudo apt update
sudo apt install sqlite3

# Install MySQL (macOS with Homebrew)
brew install mysql

# Install PostgreSQL (macOS with Homebrew)
brew install postgresql

# Install SQL Server (Docker)
docker pull mcr.microsoft.com/mssql/server:2019-latest
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=YourPassword" -p 1433:1433 mcr.microsoft.com/mssql/server:2019-latest
```

## Running SQL Programs

```bash
# MySQL client connection
mysql -u username -p database_name

# PostgreSQL client connection
psql -U username -d database_name

# SQLite connection
sqlite3 database.db

# Execute a SQL script in MySQL
mysql -u username -p database_name < script.sql

# Execute a SQL script in PostgreSQL
psql -U username -d database_name -f script.sql

# Execute a SQL script in SQLite
sqlite3 database.db < script.sql

# Execute a SQL script in SQL Server (using sqlcmd)
sqlcmd -S server_name -U username -P password -d database_name -i script.sql

# Export data (MySQL)
mysqldump -u username -p database_name > backup.sql

# Import data (MySQL)
mysql -u username -p database_name < backup.sql
```

## Common Libraries/Tools

- **Query Languages**: SQL, PL/SQL, T-SQL, PL/pgSQL
- **ORM Tools**: Hibernate, Entity Framework, Sequelize, SQLAlchemy
- **Migration Tools**: Flyway, Liquibase, Alembic
- **Data Modeling**: MySQL Workbench, ERwin, pgModeler
- **Connection Pooling**: HikariCP, c3p0, DBCP
- **Performance Monitoring**: Slow Query Log, Explain Plan
- **ETL Tools**: Apache NiFi, Talend, SSIS
- **BI & Visualization**: Tableau, Power BI, Metabase
- **Database Versions**:
  - MySQL: 5.7, 8.0
  - PostgreSQL: 12, 13, 14
  - SQL Server: 2017, 2019, 2022
  - Oracle: 18c, 19c, 21c
  - SQLite: 3.x
