# python_scripts_research
Python scripts that are used through my various research projects

## Calc_ElasticModuli_from_VTK
This script performs a volume average of elemental stress and strain quantities to determine directional elastic moduli from uniaxial strain simulations.

In this particular case, the input data is stored in VTK file format.  Simulations were performed with loading in the x-, y-, and z-directions.  The elastic moduli were calculated for each loading direction.

Elastic moduli are calculated from uniaxial stress boundary conditions, so the stiffness matrix components were first computed, then inverted to find the compliance matrix, and then the elastic moduli are determined.
