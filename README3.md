# 🚀 Oracle 21c Multitenant Lab
### PDB Lifecycle Management & Administration 🛠️

Welcome to the documentation for **Assignment II** of the **INSY 8311 - Database Development with PL/SQL** course. This repository showcases hands-on work with Oracle 21c Multitenant Architecture.

---

## 👨‍🎓 Student Spotlight
- **Name:** CYUSA Chaste
- **ID:** 29671
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

- **PDB Identity:** `ch_pdb_29671`
- **Root Admin:** `pdbadmin`
- **Local Dev User:** `chaste_plsqlauca_29671`

**Steps Taken:**
1. Logged into the CDB as `SYS`.
2. Created the `ch_pdb_29671` pluggable database.
3. Activated the PDB (switched status to OPEN).
4. Created a dedicated user for PL/SQL development inside the PDB.
5. Granted necessary roles to ensure the user can create tables and run queries.

> [!TIP]
> Always verify your container context using `show con_name` before running administrative commands!

---

### 🗑️ Task 2: Testing PDB Lifecycle (Create & Drop)
A demonstration of how to spin up and tear down temporary environments.

1. **Provisioned:** Spun up `ch_to_delete_pdb_29671`.
2. **Validated:** Verified it appears in the database list.
3. **Shutdown:** Closed the PDB safely.
4. **Clean up:** Dropped the PDB and deleted its datafiles from the disk.

---

### 📊 Task 3: Visual Management (EM Express)
Used the built-in Oracle Enterprise Manager Express to monitor the system.

- **URL:** `https://localhost:5500/em`
- **Goal:** Confirmed that all PDBs are running correctly and inspected the instance performance.

---

## 📁 What's Inside?
```bash
.
├── README.md         # Original documentation
├── README2.md        # Technical report version
├── README3.md        # This guide (Modern version)
└── Screenshots/      # Visual evidence of all tasks
    ├── ... (Evidence files 1-8)
```

---

## 📜 Legal & Integrity
This project follows strictly the academic integrity guidelines. All work was performed manually on my local Oracle instance. 

**Independent Work Verified by:** CYUSA Chaste  
**Date:** February 16, 2026

---
*Created for INSY 8311 – AUCA*
