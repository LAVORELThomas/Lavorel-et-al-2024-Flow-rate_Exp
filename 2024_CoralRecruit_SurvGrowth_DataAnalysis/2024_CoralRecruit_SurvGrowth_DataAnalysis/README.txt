Data description for 2024_FlowExpRecruit_Data.zip

This collection consists of a series of data sets assessing the sensitivity of 1-week-old recruits of the coral Acropora abrolhosensis to a gradient of flow velocities. Data was collected through laboratory experiments performed at the Australian Institute of Marine Science Townsville site following the autumn coral spawning event in Ferbuary of 2024. The data was analysed using Bayesian dose-response modelling using the package bayesnec in the software R.
Chemical analysis xls files are also included (DIN and DOC), only the first fews measurement have been included, other are still in process.

For .rmd-scripts used in analysis and further details on data wrangling for analysis please refer to https://github.com/MNordborg/Nordborg-et-al.-2022-Recruit-HFO.

Shared parameters across data files:
	Date = First day of data collection
	Exp_ID = Identification key for analysis
	Species = Recruit species used in the experiment (none in the 2024_Velocities_FlowExp)
	Flume_Nb = Flume number (Equivalent to true replicates number)
	Position_Width = Position of the coral or the coral patch in the width of the flume, letter going from A to G 
	Position_Length	= Position of the coral or the coral patch in the length of the flume, letter going from 1 to 71

Survival:
	Nb_Ind_250324 = Number of recruits dead or alive counted on the 25th of March 2024
	Nb_Dead_250324 = Number of dead recruits counted on the 25th of March 2024
	Nb_Dead_130524 = Number of dead recruits counted on the 13th of May 2024
	Survival_7weeks = Recruits survival pourcentage at 7 weeks from the start of the experiment given by the following calculation : ((Nb_Ind_250324 - Nb_Dead_130524 + Nb_Dead_250324)/ Nb_Ind_250324) * 100
	Viable_data = Qualitative data (Yes/No) giving the viability of the data

Growth:
	Photo_Nb = Gives an indication on the position of the photo in the flume. 8 photos have been taken for each flumes, the first one start at the bottom of the flume, the 8th is a photo of the top of the ramp
	px_per_mm = Gives the number of pixel for one mm, which depends on the Photo_Nb
	ROI_Nb = For each Photo_nb, each patch of coral measured is saved as a Region Of Interest, it can also be seen as the coral patch ID. Starting from 1 for each Photo_nb
	Surface_measured_px_ 250324 = Surface measure in Fiji software for each of recruit or patch of recruit the 25th March 2024, result in pixel
	Surface_measured_px_240424 = Surface measure in Fiji software for each of recruit or patch of recruit the 24th April 2024 in the flume 1. Result in pixel
	Surface_measured_px_130524 = Surface measure in Fiji software for each of recruit or patch of recruit the 13th May 2024, result in pixel 
	Surface_calculated_mm2_250324 = Surface calculated from px_per_mm and Surface_measured_px_250324 giving the result in mm2
	Surface_calculated_mm2_240424 = Surface calculated from px_per_mm and Surface_measured_px_240424 giving the result in mm2
	Surface_calculated_mm2_130524 = Surface calculated from px_per_mm and Surface_measured_px_130524 giving the result in mm2
	Growth_1month = Relative growth calculated using the following equation: (Surface_measured_mm_240424 - Surface_measured_mm_250324) / Surface_measured_mm_250324
	Absolute_Growth_1month = Relative growth over the exposure period, Growth_1month where all negative values (i.e. observed mortality) were set to 0.
	Growth_7weeks = Relative growth calculated using the following equation: (Surface_measured_mm_130524 - Surface_measured_mm_250324) / Surface_measured_mm_250324
	Absolute_Growth_7weeks = Relative growth over the exposure period, Growth_7weeks where all negative values (i.e. observed mortality) were set to 0.
	Viable_data = Qualitative data (Yes/No) giving the viability of the data