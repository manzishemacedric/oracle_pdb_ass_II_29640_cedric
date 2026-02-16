# 🚀 Oracle 21c Multitenant Lab
### PDB Lifecycle Management & Administration 🛠️

Welcome to the documentation for **Assignment II** of the **INSY 8311 - Database Development with PL/SQL** course. This repository showcases hands-on work with Oracle 21c Multitenant Architecture.

---

## 👨‍🎓 Student Spotlight
- **Name:** MANZI SHEMA Cedric
- **ID:** 29640
- **Course:** INSY 8311 (PL/SQL Development)
- **Instructor:** Eric Maniraguha

---

## 💻 Tech Stack & Setup
| Component | Details |
| :--- | :--- |
| **Engine** | Oracle Database 21c Enterprise |
| **Architecture** | CDB (Container) & PDB (Pluggable) |
| **Management** | SQL Developer, CMD, EM Express |
| **OS** | Windows |

---

## 🎯 Key Learning Objectives
- ✅ Deploying and configuring Pluggable Databases.
- ✅ Managing container contexts efficiently.
- ✅ Handling local user security and privileges.
- ✅ Monitoring database health via EM Express dashboard.
- ✅ Clean decommissioning of temporary database instances.

---

## ⚡ Task Walkthrough

### 🛠️ Task 1: Building the Core PDB
In this phase, I set up the main work environment for future development.

- **PDB Identity:** `msc_pdb_29640`
- **Root Admin:** `pdbadmin`
- **Local Dev User:** `manzi_plsqlauca_29671`

**Steps Taken:**
1. Logged into the CDB as `SYS`.
2. Created the `msc_pdb_29671` pluggable database.
3. Activated the PDB (switched status to OPEN).
4. Created a dedicated user for PL/SQL development inside the PDB.
5. Granted necessary roles to ensure the user can create tables and run queries.

> [!TIP]
> Always verify your container context using `show con_name` before running administrative commands!

---

### 🗑️ Task 2: Testing PDB Lifecycle (Create & Drop)
A demonstration of how to spin up and tear down temporary environments.

1. **Provisioned:** Spun up `msc_to_delete_pdb_29640`.
2. **Validated:** Verified it appears in the database list.
3. **Shutdown:** Closed the PDB safely.
4. **Clean up:** Dropped the PDB and deleted its datafiles from the disk.

---

### 📊 Task 3: Visual Management (EM Express)
Used the built-in Oracle Enterprise Manager Express to monitor the system.

- **URL:** `https://localhost:5500/em`
- **Goal:** Confirmed that all PDBs are running correctly and inspected the instance performance.

---


## 📜 Legal & Integrity
This project follows strictly the academic integrity guidelines. All work was performed manually on my local Oracle instance. 
 




