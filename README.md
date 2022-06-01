# Decorrelation-Timescale
This code will reads in CESM2 piControl tas-data, finds the best-fit AR(p) model for grid-point data based on Yule-Walker. The predictability timescale is estimated from the corresponding theortical autocorrelation function (ACF) in terms of metric called T2. For details on the T2, refer to DelSole (2001): https://journals.ametsoc.org/view/journals/atsc/58/11/1520-0469_2001_058_1341_oppitv_2.0.co_2.xml
Note, this estimate of predictability is made for data where there is no climate change signal. When analizing data with external forcings (GHG, aersols, etc.) this signal should be removed prior to fitting the AR(p) model.
Estimates of the best-fit AR(p) model for grid-point data are based on Yule-Walker equations and are contained in arfit_yw.py 
