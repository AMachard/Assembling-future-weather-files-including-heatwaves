# Assembling-future-weather-files-including-heatwaves

To use this code, please cite the following publication:

Machard, A. , Inard, C., Alessandrini, J.M., Pelé, C., Ribéron, J.
A Methodology for Assembling Future Weather Files Including Heatwaves for Building Thermal Simulations from the European Coordinated Regional Downscaling Experiment (EURO-CORDEX) Climate Data
https://doi.org/10.3390/en13133424

The objective of this code is to use CORDEX climate projections to create future weather files as input for building thermal simulations. These future weather files can either be typical years (TMY) either years containing heatwaves (HWY).
These climate projections can also be used for other purposes.

This code is composed into 3 parts.

Part I : This code extracts CORDEX future climate data projections from NETCDF4 files and converts them into CSV at hourly format. It uses 12 NETCDF4 files as examples (2 years for 6 weather variables) needed for building thermal simulations. 
The 12 examples files are described here and must be downloaded from the CORDEX Platform https://cordex.org/
These files need to be added to the folder "Part-I_ExampleFiles"
![image](https://user-images.githubusercontent.com/112181707/200349373-8457664b-a28a-4f52-98e2-ca238705d8b0.png)

The user must download all CORDEX files from multi-year (30 years recommended for minimum 4 weather variables: tas, hurs, rsds, sfcWind) to proceed to Part II & Part III. It is also advised that the user proceed to bias-correct the multi-year projections over the reference period using climate observations before proceeding to Part II & Part III, especially for heatwave detection.

Part II : This code uses multiyear climate projections to create a typical year following the norm EN 15251-4.

Part III : This code uses multiyear climate projections to select heatwaves.

Part II & Part III use the example files attached here:
[Multiyears-BC_Roissy_MPI-RCA4_2010s.zip](https://github.com/AMachard/Assembling-future-weather-files-including-heatwaves/files/9953075/Multiyears-BC_Roissy_MPI-RCA4_2010s.zip) and
[Multiyears-BC_Roissy_MPI-RCA4_2050s.zip](https://github.com/AMachard/Assembling-future-weather-files-including-heatwaves/files/9953110/Multiyears-BC_Roissy_MPI-RCA4_2050s.zip)
These files need to be added to the folder "Part-II-and-Part-III_ExampleFiles"


