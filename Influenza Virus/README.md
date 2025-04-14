This folder contains the simulation setup, configuration files, and results for the molecular dynamics (MD) simulation of Influenza Virus (2YP2).
# 🧬 MD Simulation of Influenza Virus (2YP2)

This folder contains the simulation setup, configuration files, and results for the molecular dynamics (MD) simulation of **Influenza Virus (PDB ID: 2YP2)** using [GROMACS](http://www.gromacs.org/).

---

## 📁 Folder Contents

| Folder/File            | Description                                          |
|------------------------|------------------------------------------------------|
| `input_files/`         | Topology, coordinates, and force field parameters    |
| `equilibration/`       | Equilibration steps (NVT, NPT)                       |
| `production/`          | Production run outputs                               |
| `analysis/`            | Trajectory analysis scripts and results              |
| `2YP2.pdb`             | Original PDB structure from RCSB                     |
| `README.md`            | This documentation                                   |

---

## ⚙️ Simulation Details

- **Software used:** GROMACS 2023
- **Force field:** CHARMM36
- **Water model:** TIP3P
- **Simulation box:** Cubic box with 1.0 nm padding
- **Ions added:** Na⁺ and Cl⁻ to neutralize the system
- **Temperature:** 300 K (NVT)
- **Pressure:** 1 bar (NPT)
- **Time step:** 2 fs
- **Total simulation time:** 100 ns

---

## 🧪 Workflow Overview

1. **System Preparation**
   - Retrieved 2YP2 from RCSB
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

- **RMSD & RMSF**
- **Radius of gyration**
- **Hydrogen bond analysis**
- **SASA (Solvent Accessible Surface Area)**
- **Secondary structure analysis (DSSP)**

---

## 📝 Notes

- Make sure to load the correct version of GROMACS before running scripts.
- All `.mdp` configuration files are available in respective subfolders.

---

## 📎 References

- RCSB PDB: [https://www.rcsb.org/structure/2YP2](https://www.rcsb.org/structure/2YP2)
- CHARMM36: [https://mackerell.umaryland.edu/charmm_ff.shtml](https://mackerell.umaryland.edu/charmm_ff.shtml)

---

## 👩‍💻 Author

**Liza** – Researcher in Molecular Simulations & Photonics  
For questions, contact via GitHub or [LinkedIn](#)

