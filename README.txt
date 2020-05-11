# MitoWave
Spatio-Temporal Mitochondrial membrane potential fluctuation Analysis during Ischemia Reperfusion

This routine requires switching between ImageJ(OR FIJI) and MATLAB.
Language written for ImageJ is ImageJ Macro or .ijm. It can be copy pasted to run on FIJI. 
Comments and annotations are after  '//' or '%%'. 
Modifications must be made if sampling rate is different from what we used. We sampled at the rate of 1 image every 15 seconds to get 241 images in a period of 60.25 minutes. 
Arrays containing required data for Ischemia ΔΨm depolarization time, Average frequency of each cell, mitochondrial frequencies and associated timepoints, mitochondrial cluster areas, mitochondrial ΔΨm depolarization time, cellular depolarization time are described below. 

FINAL RESULTS ARE IN THE FOLLOWING ARRAYS:

IPT_2MAT_Depolarization_minutes – Has the time point at which a cell depolarized during Ischemia 

cell_classification – Column 1 has the state of each cell at the beginning of reperfusion, Column 2 has the time at which the cell depolarized (based on if 60% of mitochondria depolarized in that cell), Column 3 has the average frequency of that cell (based on average frequency of the oscillating clusters)

death_timefornotdeadmito_minutes – Has the timepoint at which a mitochondrial cluster exhibited irreversible ΔΨm depolarization during Reperfusion

Freqconvertedfromscale_MITO- Has the average frequency of a mitochondrial cluster separated into different frequency bands and associated with a particular timepoint during reperfusion. Column 1 has frequencies ranging from 8.6-45mHz, Column 2 has 8.6-4.3mHz, Column 3 has 4.3-3mHz, Column 4 has 3-2.2 mHz, Column 5 has 2.2-1.8mHz and Column 6 has frequencies below 1.8 mHz. 

Freq_associated_time_minutes - Has the timepoint associated with the particular frequency of a mitochondrial cluster. Column 1 has frequencies ranging from 8.6-45mHz, Column 2 has 8.6-4.3mHz, Column 3 has 4.3-3mHz, Column 4 has 3-2.2 mHz, Column 5 has 2.2-1.8mHz and Column 6 has frequencies below 1.8 mHz. Along with the ΔΨm depolarization time, these values are used to make the violin plots to obtain a complete graphical visualization of the dynamic oscillatory behavior of mitochondrial ΔΨm. 

MitoAreasArray – Contain area of each mitochondrial cluster

Freq_MITO – Has the predominant frequency exhibited by the mitochondrial cluster
