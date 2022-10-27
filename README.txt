Included in the assignment .zip are 4 distinct rosette casts, with 4 files associated with each cast. The casts are labeled in order with the notation SSSCC, where SSS is the Station number and CC is the Cast number (at that specific station). 

The 4 files per cast are:

* *.cnv - The continuous CTD data from the entire cast in scientific units at 24 Hz (native sampling frequency).
* *.btl - The bottle summary file contains upcast CTD data averaged at each bottle trip. These data should be fit to reference temperature and salinity.
* *.cap.btl_t - The reference thermometer data file holds the "true" temperature to fit against. T90 is the column with temperature, bottle_number is the column that tells you the associated bottle.
* *.lst - The reference salt data file with the "true" salinity to fit against. You will want the "avg cr" or the salt value from this file.

For the assignment, we would like you to do as much of the following as possible, to the best of your ability:

1. Inspect and import the data files.
2. Plot the continuous CTD data and identify the mixed layer depth, the thermocline and halocline, relevant minima and maxima, and anything else of interest.
3. Fit the raw temperature data (.btl) to the reference thermometer (.cap.btl_t) as a function of pressure using any method of your choosing.
4a. Convert the salt data file (.lst) from "conductivity ratio" or salinity to conductivity (this is your "true"/reference conductivity).
4b. Fit the raw conductivity data (.btl) to the reference conductivity as a function of pressure using any method of your choosing.
5. Apply the temperature/conductivity fit to the continuous CTD data (.cnv).
6. Plot the corrected/fitted data. Compare with the raw data and describe the results.

To be explicit, there should be at least one of the following plots available for review:
– Continuous temperature vs. pressure
– Continuous conductivity vs. pressure
– Continuous temperature fitted to discrete temperature vs. pressure
– Continuous conductivity fitted to discrete conductivity vs. pressure
– Continuous salinity fitted to discrete salinity vs. pressure

While we will accept solutions in any language, Python is the language used in the group and is preferred for the assignment. Please be prepared to present and discuss the results during the interview - Jupyter notebook preferred if in Python, Julia, or R.

For converting the conductivity ratio or salinity to conductivity, you can use Gibbs SeaWater Oceanographic Toolbox of TEOS-10, of which there are libraries for Matlab and Python, and possibly other languages.
https://pypi.python.org/pypi/gsw/
http://www.teos-10.org/pubs/gsw/html/gsw_contents.html

For additional guidance on general oceanographic processing methods you can refer to the GO-SHIP manual, found at http://www.go-ship.org/HydroMan.html You will not be penalized if you do not follow the guidelines in the manual.

Finally, feel free to look at our group's Python package "ctdcal", found at http://www.github.com/cchdo/ctdcal As with the GO-SHIP manual, you will not be penalized for not using ctdcal.

Please complete as much as possible prior to the interview. We do not necessarily expect you to complete all 6 steps for all stations before turning in the assignment. We hope you spend around an hour on the problems, and expect to have a discussion about your progress – if you have any questions feel free to bring them.
