<p align="left">
  <img src="img/liquibase.png" alt="Liquibase Logo" title="Liquibase Logo" width="324" height="72">
</p>

# 👋 Welcome to Liquibase!
Liquibase Secure (formerly Liquibase Pro) is database change management made easy. This repository contains sample changelogs organized by object type and release.

# 📖 Overview
This repository provides two sample Liquibase changelog structures for your database deployment needs.
* Object Type Organization - Changelogs grouped by database object type (tables, views, stored procedures, etc.)
* Release Version Organization - Changelogs grouped by release version for sequential deployment tracking

The initial changesets were built using the [Adventure Works 2019](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms) database provided by Microsoft for SQL Server. The file structure is correct and intended as a reference. However, the changelogs will not run as-is due to missing dependencies (only a subset of objects are included).

Best practices for changelog management can be found [here](https://docs.liquibase.com/secure/implementation-guide-5-0).

# 📂 Directory By Object
```
changelog.type.xml
├───Tables
│       Person.Person.sql
│       Purchasing.Vendor.sql
│       Sales.Customer.sql
├───Views
│       HumanResources.EmployeeDepartmentHistory.sql
│       Purchasing.VendorWithAddress.sql
│       Sales.StoreWithContacts.sql
├───Stored Procedures
│       HumanResources.UpdateEmployeeLogin.sql
│       SalesTopTen.sql
│
```

# 📂 Directory By Version
```
changelog.version.xml
├───Version 1.0
│       version1_0.sql
├───Version 1.1
│       version1_1.sql
```

# 🤔 Which Should I Use?
* **Object Type** - Best for organizing changes by database structure (tables, views, stored procedures, etc.). Useful when different team members own different object types or when you want to find all changes to a specific type of object quickly.

* **Release Version** - Best for organizing changes by when they'll be deployed. Useful for tracking what goes out together in each release and maintaining clear deployment history.

**Note!** Either approach is valid, or combine them! Liquibase does not impose any structural requirements.

# ☎️ Contact Liquibase
Liquibase sales: https://www.liquibase.com/contact-us<br>

# ⭐ Thank you!
Thank you for evaluating Liquibase Secure! We hope to be a part of your DevOps journey.