# newspace-ursamajor-astrodynamics

Relevant Basilisk files for NewSpace @ Berkeley's Astrodynamics project for Ursa Major (2025-2026).

> **Note:** Basilisk must be downloaded and placed appropriately before running any simulation code.
> Download link and official documentation: [https://avslab.github.io/basilisk/](https://avslab.github.io/basilisk/)

---

## Requirements

**`requirements.txt`** — All necessary Python dependencies, including those required by Basilisk.

---

## File Structure

```
newspace-ursamajor-astrodynamics/
├── requirements.txt
├── hohmanntransfers/
│   ├── hohmannBasiliskexample.py
│   └── hohmanntransfertest.py
├── highthrustsimulations/
│   └── basiliskhighthrust.py
└── lowthrustsimulations/
    ├── basilisklowthrust.py
    └── csv_saving_basilisklowthrust.py
```

---

## Modules

### `hohmanntransfers/`
Simulation code for modeling ideal (impulsive burn) Hohmann transfers.

| File | Description |
|------|-------------|
| `hohmannBasiliskexample.py` | Basilisk's official Hohmann transfer example. Demonstrates the necessary syntax and simulation framework for designing a mission in Basilisk. |
| `hohmanntransfertest.py` | Hohmann transfer simulation without Basilisk. Uses core physical equations (Vis-Viva, etc.) only. |

---

### `highthrustsimulations/`
Simulation code for modeling chemical propulsion systems (discrete burns).

| File | Description |
|------|-------------|
| `basiliskhighthrust.py` | Models high-thrust (chemical) propulsion systems. Configure initial and target altitudes, total satellite mass, and thruster parameters before running. |

---

### `lowthrustsimulations/`
Simulation code for modeling electric propulsion systems (continuous burns).

| File | Description |
|------|-------------|
| `basilisklowthrust.py` | Models low-thrust (electric) propulsion systems. Configure initial and target altitudes, total satellite mass, and thruster parameters before running. |
| `csv_saving_basilisklowthrust.py` | Same as above, with post-simulation CSV export for downstream analysis. |
