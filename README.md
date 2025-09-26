# ATMS-523-Module-2 Project

This code uses xarray and dask to manage ERA-5 total precipitation (from google cloud) files.
The city of Valparaiso, Indiana is chosen as a starting point for initial time series analysis.

# Why Valparaiso?
Valparaiso was chosen due to its unique location near Lake Michigan, which puts Valparaiso in the vicinity of
several lake-breeze boundaries throughout the year which act as triggers for convection. 

# Figure 1
The first analysis is a simple time series from 1990-2020 showing daily precipitation for both a point in Valparaiso
and a 5x5 degree grid-box with Valparaiso at the center. As expected, the gridbox has some lower values than the singular point
in the center of town.

# Figure 2
The second analysis shows a cumulative distributive function of all values in the time with the point of the 95th percentile
marked in red. 

# Figure 3
The third analysis shows what is happening in the rest of CONUS when Valparaiso has a 95th percentile event. Both a composite plot
and an anomaly plot are shown. In general, the Midwest is heavily impacted by these events but other portions of the CONUS remain
relatively dry. These days could predominantly be the cause of mid-latitude cyclones bringing in fronts and Mesoscale-convective systeme
that bring high amounts of precipitation. These events that impact Valparaiso would mostly be impacting the Midwest and not anywhere else. 

# References
Carver, Robert W, and Merose, Alex. (2023):
ARCO-ERA5: An Analysis-Ready Cloud-Optimized Reanalysis Dataset.
22nd Conf. on AI for Env. Science, Denver, CO, Amer. Meteo. Soc, 4A.1,
https://ams.confex.com/ams/103ANNUAL/meetingapp.cgi/Paper/415842

Hersbach, H., Bell, B., Berrisford, P., Hirahara, S., Horányi, A., 
Muñoz‐Sabater, J., Nicolas, J., Peubey, C., Radu, R., Schepers, D., 
Simmons, A., Soci, C., Abdalla, S., Abellan, X., Balsamo, G., 
Bechtold, P., Biavati, G., Bidlot, J., Bonavita, M., De Chiara, G., 
Dahlgren, P., Dee, D., Diamantakis, M., Dragani, R., Flemming, J., 
Forbes, R., Fuentes, M., Geer, A., Haimberger, L., Healy, S., 
Hogan, R.J., Hólm, E., Janisková, M., Keeley, S., Laloyaux, P., 
Lopez, P., Lupu, C., Radnoti, G., de Rosnay, P., Rozum, I., Vamborg, F.,
Villaume, S., Thépaut, J-N. (2017): Complete ERA5: Fifth generation of 
ECMWF atmospheric reanalyses of the global climate. Copernicus Climate 
Change Service (C3S) Data Store (CDS). (Accessed on 25-09-2025)
