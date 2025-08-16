# SRIM Post-Processing: Cesium Implantation in UO₂

This repository contains a Python script to post-process SRIM (Stopping and Range of Ions in Matter) output files for Cesium (Cs) implantation in Uranium Dioxide (UO₂). The script calculates the atomic concentration profile and the damage (dpa) profile from SRIM results.

## Features

Reads SRIM exported data files:

IonDistribution.txt: Cesium ion distribution vs depth

VacancyProfile.txt: Vacancy profile vs depth

Converts depth from Ångström to nanometers.

## Calculates:

Cesium atomic concentration in atomic %.

Displacements per atom (dpa) profile.

### Generates a dual-axis plot:

Left axis: Cesium concentration ([Cs] in at.%)

Right axis: dpa profile

## Usage

Place the SRIM output files (IonDistribution.txt and VacancyProfile.txt) in the same directory as the script.

### Adjust parameters in the script if needed:

- fluence: ion fluence (ions/cm²)

- rho: material density (g/cm³)

- M: molar mass of the host material (g/mol)

- fm: mass fraction factor for the host material

## Run the script:

- python3 dpaConsDepth.py


The script will produce a plot showing the Cs concentration and dpa profile as a function of depth.

## Example in the image

The provided example uses:

- Fluence: 1e15 ions/cm²

- Material: Uranium Dioxide (UO₂)

- Depth axis converted from Å to nm

Plots [Cs] in atomic % vs depth and dpa profile on a secondary axis# SRIM_Implantation_dpa_Conscentration_depth