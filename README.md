# Lavorel-et-al-2024-Flow-rate_Exp
This collection consists of a series of data sets assessing the water flow velocity of three modified 100mm by 100 mm flumes. Modifications consist of additional ramp and fences inside each flume. Data was collected through laboratory experiments performed at the Australian Institute of Marine Science Townsville site in February. The data was collected from IDS camera records and analyse using PIVLab in Matlab software. The data results in three matrix Matlab (.mat) corresponding to the three flumes. These matrix are analyzed using R software.

Description of data files:
	2024_CFDVelocities_FlowExp: a .xlsx file including flow measurements made using Autodesk CFD
	2024_Velocities_FlowExp: a .Rmd files linked to the CFD_Simulation_Script R.proj file, including the data treatment of the different files included in the folder
	Flume1.mat, Flume2.mat and Flume3.mat: three matrix files from Matlab including the velocity of flumes calculated with PIVLab.

.mat files:
	The matrices represent the surface of the measurement area, the columns from A to G represent the width position of the measurement and the rows going from 1 to 71 represent the length position of the measurement (we can consider these matrices as heat maps of velocity)

2024_CFDVelocities_FlowExp:
	Length_Units: correspond to the y coordinates in Autodesk following the ramp
	Velocity_CFD: expressed in cm s-1, its represent the velocity associated to the length unit 
