#Seismic Hazard Assessment using Monte Carlo Simulation

Statistics of significant earthquakes (Mw ≥ 5.0 and distance ≤ 400 km) are established for a building in Metro Manila based on an earthquake catalog in the past 122 years. Seismic hazard assessment utilizing conventional Probabilistic Seismic Hazard Analysis (PSHA) may be validated using the Monte Carlo Simulation (MCS) method and this notebook presents a framework for performing MCS in Python for seismic hazard assessments. The seismicity of the project site is determined through descriptive statistics of various earthquake parameters which will also serve as input variables for the simulation. This notebook will also highlight common methods, function calls, and visualization tools that are important in statistical studies and random sampling methods.

The following libraries were used in the simulation:

* Numpy, Scipy, Math - mainly used to handle statistical models, mathematical computations, and random number generators for the simulation
* Pandas - data manipulation and storage of multi-dimensional arrays
* Folium, Seaborn, Matplotlib - data visualization of geographical distribution, histograms, probability mass function, and cumulative distribution function of random variables

The United States Geological Survey (USGS) is an agency that monitors natural hazards around the world including earthquakes and the data used in this study were downloaded from their [database](https://earthquake.usgs.gov/earthquakes/).

The figures below show the histograms and distribution of various parameters.
