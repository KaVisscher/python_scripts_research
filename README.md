# Python Scripts Used For Research Purposes
This repository contains Python scripts that I have created at some point during my research endeavor.  I thought it would be nice to publish and, more importantly, document them and if others benefit, then great.  These codes are somewhat simplistic in nature, meaning they hopefully aren't too long.  

The purpose is for the directories to be self-containing with all required input files, codes, and any example outputs you can expect from the code in current form.

## Determining Elastic Moduli from Uniaxial Strain FEM Data
#### Calc_ElasticModuli_from_VTK
This script performs a volume average of elemental stress and strain quantities to determine directional elastic moduli from uniaxial strain simulations.

In this particular case, the input data is stored in VTK file format.  Simulations were performed with loading in the x-, y-, and z-directions.  The elastic moduli were calculated for each loading direction.

Elastic moduli are calculated from uniaxial stress boundary conditions, so the stiffness matrix components were first computed, then inverted to find the compliance matrix, and then the elastic moduli are determined.

## Reading and Writing VTK files
This script illustrates how to read and write VTK file formats that include scalar, vector, and tensor data.  

## Plotting Stress-Strain Curves from FEM data 
This script reads in force and displacement data from Abaqus .dat files and generates an engineering stress-strain curve.