# 🧬 # MD Simulation of Gallus gallus (1AKI)

This folder contains the simulation setup, configuration files, and results for the molecular dynamics (MD) simulation of **Influenza Virus (PDB ID: 2YP2)** using [GROMACS](http://www.gromacs.org/).

---

## 📁 Folder Contents

| File                   | Description                                          |
|------------------------|------------------------------------------------------|
| `input_files`         | Topology, coordinates, and force field parameters    |
| `equilibration`       | Equilibration steps (NVT, NPT)                       |
| `production`          | Production run outputs                               |
| `analysis`            | Trajectory analysis scripts and results              |
| `2YP2.pdb`             | Original PDB structure from RCSB                     |
| `README.md`            | This documentation                                   |

---

## ⚙️ Simulation Details

- **Software used:** GROMACS 2023
- **Force field:** OPLSAA force field
- **Water model:** TIP3P
- **Total simulation time:** 100 ns

---

## 🧪 Workflow Overview

1. **System Preparation**
   - Retrieved 1AKI from RCSB
   - Cleaned structure and added missing atoms

2. **Topology Generation**
   - Generated topology using `pdb2gmx`
   - Defined box and solvated the system

3. **Energy Minimization**
   - Steepest descent algorithm

4. **Equilibration**
   - NVT (100 ps) and NPT (100 ps) with position restraints

5. **Production MD**
   - 100 ns unrestrained MD run

---

## 📊 Analysis Performed

- **RMSD**
- **RMSF**
- **Radius of gyration**



---

## 📝 Notes

- Make sure to load the correct version of GROMACS before running scripts.


---

##  References

- RCSB PDB: [https://www.rcsb.org/structure/2YP2](https://www.rcsb.org/structure/1AKI)
- 

---

## 👩‍💻 Author
Elizebeth Lyngdoh Nonglait

