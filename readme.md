# README

This repository contains data tables related to energy consumption and availability experiments in a read/write operations. Below are the descriptions of the tables and their respective fields.

---

## **filename:** `availability_experiment_dataset.csv`

**Columns:**
1. **cons**  
   - A factor that may represent consistency level.
2. **RF**  
   - Replication factor.
3. **Proportion (leitura / escrita)**  
   - The proportion of read/write operations (e.g., `0.8 read / 0.2 write`).
4. **replica MTTF (failure sw)**  
   - Mean Time To Failure (MTTF) of the replica, in hours (average time until failure).
5. **replica MTTR (restore sw)**  
   - Mean Time To Repair (MTTR) of the replica, in hours (average repair time).
6. **Esys (J)**  
   - Total energy consumption in Joules.
7. **availability **  
   - System availability.
---

## **filename:** `workload_variation_experiment_dataset.csv`

**Columns:**
1. **cons**  
   - Consistency level (similar meaning as in Table 1).
2. **RF**  
   - Replication factor.
3. **proportion (read / write)**  
   - Read/write operation proportion.
4. **Pread (J/s)**  
   - Average power consumption for read operations, in Joules per second.
5. **Pwrite (J/s)**  
   - Average power consumption for write operations, in Joules per second.
6. **Eread (J)**  
   - Total energy consumed by read operations, in Joules.
7. **Ewrite (J)**  
   - Total energy consumed by write operations, in Joules.
8. **Esys (J)**  
   - Sum of read and write energy, in Joules.

---


## **filename:** `performability_model.xml`

This file contains the performability model created using TimeNet 4.5.
---

## Observations

- MTTF and MTTR values might be on different hour scales, depending on the experiment.
- Make sure to confirm the units (e.g., hours for time, Joules for energy) before performing any analysis or comparisons.

---

If you have any questions or suggestions, feel free to open an issue or get in touch. Thank you for checking out our repository!