Data for the StatsLab project, downloaded from https://sensors-eawag.ch/sars/overview.html on March 2 2022.

Files are as such: processed_normed_data_<city>_<version>.csv , where <city> refers from the city of the surveyed WWTP, and <version> is either v1 or v2, and refers to the protocol used. The first part of the time series was generated with the first protocol, and the second part with the second, with an overlap in between. More info about the difference between protocols can be found on https://sensors-eawag.ch/sars/overview.html. 

Time series for Lausanne stops in Summer 2021, when monitoring was switched to surveying the WWTP in Lausanne to the one in Geneva. For this reason, all of Lausanne samples were treated with only one version of the protocol and there is only one csv. The time series for Geneva starts in Summer 2021. 

Files have columns:
	- sars_cov2_rna [gc/(d*100000 capita)]
		Daily SC2 RNA concentrations, normalised by population
	- median_7d_sars_cov2_rna [gc/(d*100000 capita)]
		Same but smoothed with running median
	- new_cases [1/(d*100000 capita)]
		Normalised new cases in the catchment area of the WWTP
	- median_7d_new_cases [1/(d*100000 capita)]
		Same as above with smoothed with running median
	- quantification_flag [{Q: >LOQ,D: >LOD,N: <LOD}]
		Quantification limits of the instrument
	- flow [m^3/d]
		Flow to the WWTP