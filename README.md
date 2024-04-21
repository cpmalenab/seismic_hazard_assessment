# Seismic Hazard Assessment using Monte Carlo Simulation

Statistics of significant earthquakes (Mw ≥ 5.0 and distance ≤ 400 km) are established for a building in Metro Manila based on an earthquake catalog in the past 122 years. Seismic hazard assessment utilizing conventional Probabilistic Seismic Hazard Analysis (PSHA) may be validated using the **Monte Carlo Simulation (MCS)** method and this notebook presents a framework for performing MCS in Python for seismic hazard assessments. The seismicity of the project site is determined through *descriptive statistics* of various earthquake parameters which will also serve as input variables for the simulation. This notebook will also highlight common methods, function calls, and visualization tools that are important in statistical studies and random sampling methods.

The following libraries were used in the simulation:

* **Numpy, Scipy, Math** - mainly used to handle statistical models, mathematical computations, and random number generators for the simulation
* **Pandas** - data manipulation and storage of multi-dimensional arrays
* **Folium, Seaborn, Matplotlib** - data visualization of geographical distribution, histograms, probability mass function, and cumulative distribution function of random variables

The United States Geological Survey (USGS) is an agency that monitors natural hazards around the world including earthquakes and the data used in this study were downloaded from their [database](https://earthquake.usgs.gov/earthquakes/).

The figure below shows the effect of varying the number of trials to the smoothness of the curve.

<p align="center">
  <img src="https://github.com/cpmalenab/seismic_hazard_assessment/blob/main/images/simulation.PNG">
</p>
<p align="center">Figure. Monte Carlo Simulation with Varying Number of Trials</p>

The plot of hazard curves with varying number of years show that at lower probabilities of exceedance (more rare events), the tail end of the graph is not as defined as those with higher probabilities. Thus, a large number of samples is required to obtain more data points at the regions of lower probability.

<p align="center">
  <img src="https://github.com/cpmalenab/seismic_hazard_assessment/blob/main/images/annual%20hazard%20curves%20for%20different%20periods.PNG">
</p>

<p align="center">Figure. Annual Hazard Curves for Different Structural Periods (no. of years = 1,000,000)</p>

To view the full documentation and implementation of the project, please visit this [notebook](https://nbviewer.org/github/cpmalenab/seismic_hazard_assessment/blob/main/Seismic%20Hazard%20Assesment%20using%20Monte%20Carlo%20Simulation.ipynb) and the accompanying [research paper](https://nbviewer.org/github/cpmalenab/seismic_hazard_assessment/blob/main/Seismic%20Hazard%20Assessment%20of%20a%20Residential%20Building%20in%20Metro%20Manila%20using%20Reliability-based%20Methods.pdf).





