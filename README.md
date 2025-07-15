# Order Management System - Backup & Restore

This repository documents the backup and restore process I completed for my Order Management System database using MySQL Workbench.

## Repository Structure

```
order-management-backup-restore/
├── README.md                  # Project overview & documentation
├── Backup and Restore Process/
│   └── MySQL Workbench Backup Process
│   └── MySQL Workbench Restore Process
│   └── Microsoft SSMS Backup Process
│   └── Microsoft SSMS Restore Process  
├── Additonal info/
├── LICENSE                    # MIT License
```

## About This Project

I completed the backup of a database and successfully restored the backup into a new database instance using MySQL Workbench and Microsoft SSMS.


## Backup & Restore Process

### MySQL Workbench Backup Process

1. Open **MySQL Workbench**.
2. Go to **Server → Data Export**.
3. Select the [`order_management`](https://github.com/Kifaa-yah/Order-Management-System/blob/main/sql/order_management_schema.sql) database (see schema).
4. Choose **Export to Dump Folder**.
5. Select destination → `backup/order_management_dump/`.
6. Click **Start Export**.

### MySQL Workbench Restore Process

1. Open **Microsoft SSMS**.
2. Right clickon the database **Server → Data Import**.
3. Choose **Import from Dump Folder**.
4. Browse to the path → `backup/order_management_dump/`.
5. Select or create a **new database** → e.g., `order_management_restore`.
6. Click **Start Import**.

### Microsoft SSMS Backup Process

1. Open **Microsoft SSMS**.
2. Right click on the database in the **object explorer** 
2. Select **Tasks**.
5. Choose **Back up**.
6. In the dialogue box, choose the **Database**, select back up type **(Full)** and choose **Destination**
8. Click **Ok**.

### Microsoft SSMS Restore Process

1. Open **Microsoft SSMS**.
2. Right click the database in the **object explorer** 
2. Select **Tasks**.
5. Choose **Restore**.
6. Select **Database**
7. Chnage database name to OrderManagementDBNew (or any related name of choice) under **Destination**
8. Click **Ok**.

**Additonal info**  
During the restore, i encountered erroe message 'Restore of database **'OrderManagentDBNew' failed. (Microsoft.SqlServer.Management.RelationalEngineTasks)'**

**How to resolve it**  
    Right-click the database → Select Tasks → Restore → Database.
    In the Options tab on the left pane:
    Check "Close existing connections".
    Proceed with the restore.
   
## License

MIT License

---

Built with ❤️ by Kifaayah
