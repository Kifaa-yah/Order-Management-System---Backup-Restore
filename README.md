# 📦 Order Management System - Backup & Restore

This repository demonstrates **backup and restore** procedures for my custom-built **Order Management System** database using **MySQL Workbench**.

## 🎯 Why This Project?

* To showcase practical experience with **database backup & restore**
* To document real-life database workflows
* To improve database management skills using MySQL Workbench

## 🏗️ Project Features

* Custom-built database schema for an **Order Management System**
* Sample data included for demonstration
* Complete **backup and restore process** documented

## 📁 Repository Structure

```
order-management-backup-restore/
├── README.md                  # Project overview & documentation
├── LICENSE                    # MIT License
├── backup/
│   └── order_management_dump/  # MySQL dump folder (exported)
├── restore/
│   └── restore_instructions.md # Step-by-step restore guide
├── sql/
│   ├── order_management_schema.sql   # Database schema (CREATE TABLE)
│   └── order_management_sample_data.sql # Sample data (INSERT queries)
```

## ♻️ Backup & Restore Process

### 🔹 Backup Process

1. Open **MySQL Workbench**.
2. Go to **Server → Data Export**.
3. Select the `order_management` database.
4. Choose **Export to Dump Folder**.
5. Select destination → `backup/order_management_dump/`.
6. Click **Start Export**.

### 🔹 Restore Process

1. Open **MySQL Workbench**.
2. Go to **Server → Data Import**.
3. Choose **Import from Dump Folder**.
4. Browse to the path → `backup/order_management_dump/`.
5. Select or create a **new database** → e.g., `order_management_restore`.
6. Click **Start Import**.



## 📚 License

MIT License

---

Built with ❤️ by Kifaayah
