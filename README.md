# oracle_pdb_assignment_IZABAYO_Parfait_27144

Assignment of PDB Creation, Deletion, and Configuring Database Actions (ORDS)
 PDB Creation and Deletion Assignment
Overview

This repository documents the step-by-step process for creating and deleting a Pluggable Database (PDB) in Oracle Database 23ai Free Edition.
It also covers how to configure and access Oracle Database Actions (ORDS) — the modern replacement for Oracle Enterprise Manager (OEM Express) — to visually verify the PDB operations.

 Tasks Completed
1️ Create a Pluggable Database (PDB)

Created a new PDB named IZ_PDB_27144 using SQL*Plus.

Admin user created: IZABAYO_PLSQLAUCA_27144.

Verified that the PDB was successfully opened in READ WRITE mode.

📸 Screenshot included showing PDB list with IZ_PDB_27144.

2️⃣ Delete a Pluggable Database (PDB)

Created and opened a temporary PDB named IZ_TO_DELETE_PDB_27144.

Verified that it was active.

Closed and dropped the PDB safely using the INCLUDING DATAFILES clause.

Verified that it was successfully removed from the list of PDBs.

📸 Screenshot included before and after deletion.

3️⃣ Configure Oracle Database Actions (ORDS)

In Oracle 23ai Free Edition, OEM Express (/em) is replaced with Database Actions (/ords).

Enabled HTTPS port 5500 using:

EXEC DBMS_XDB_CONFIG.SETHTTPSPORT(5500);
EXEC DBMS_XDB_CONFIG.SETGLOBALPORTENABLED(TRUE);


Verified access via browser at:

https://localhost:5500/ords/izabayo_plsqlauca_27144/


Logged in using:

Username: izabayo_plsqlauca_27144
Password: Ora#27144


📸 Screenshot included showing the Database Actions dashboard.

📸 Screenshots

✅ Screenshot 1: PDB creation and open mode (READ WRITE).

✅ Screenshot 2: PDB deletion confirmation.

✅ Screenshot 3: Database Actions dashboard with username and database name.

📂 Resources

👉 Click here to view all project screenshots

📄 Click here to open the project report document

📚 References

Oracle Database 23c Free — Official Documentation

Oracle REST Data Services (ORDS) User Guide

Oracle Database Actions Overview
