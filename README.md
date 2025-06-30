# Order Management System - Backup & Restore

This repository documents the backup and restore process I completed for my Order Management System database using MySQL Workbench.

## Repository Structure

```
order-management-backup-restore/
├── README.md                  # Project overview & documentation
├── backup/
│   └── backupe_instructions.md # Step-by-step backup guide
│   └── order_management_dump/  # MySQL dump folder (exported)
├── restore/
│   └── restore_instructions.md # Step-by-step restore guide
├── LICENSE                    # MIT License
```


## About This Project

As part of my learning process in database management, I:

Designed and created the Order Management System database

Completed a backup of the database using MySQL Workbench

Successfully restored the backup into a new database instance

This project is a personal record of that process.


## ♻️ Backup & Restore Process

### 🔹 Backup Process

Click Start Export.
1. Open **MySQL Workbench**.
2. Go to **Server → Data Export**.
3. Select the [`order_management`](https://github.com/Kifaa-yah/Order-Management-System/blob/main/sql/order_management_schema.sql) database (see schema).
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
