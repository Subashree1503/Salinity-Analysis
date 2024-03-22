# Unveiling-Oceanic-Dynamics-Machine-Learning-Insights-into-Salinity-Variation-and-Ecosystem-Response


### Introduction:
The exploration of salinity levels in oceanic environments is fundamental in understanding the intricate dynamics of the water cycle, ocean circulation, and their implications for climate change. Salinity serves as a crucial parameter, influencing the density of seawater and thus shaping its movement and mixing patterns. The variations in salinity directly impact marine ecosystems, as many organisms have evolved to thrive within specific salinity ranges, affecting their distribution, reproduction, and overall survival.

The Conductivity, Temperature, and Depth (CTD) casts—a suite of electronic instruments is used to measure various oceanographic properties, including salinity, dissolved oxygen, chlorophyll-a, and nutrients. These measurements provide a comprehensive overview of the physical characteristics of seawater, aiding in charting its distribution and variations.

The dataset used in this study originates from the CalCOFI dataset, representing one of the longest and most extensive time series of oceanographic and larval fish data globally. Collected from over 50,000 sampling stations, this dataset offers a wealth of information on oceanographic conditions, measured through CTD casts conducted at CalCOFI stations.

In this investigation, the objective is to develop a machine learning model capable of estimating water salinity based on biochemical oceanographic measurements and the year of measurement. By harnessing the power of machine learning, the aim is to uncover the intricate relationships between various oceanographic parameters and salinity levels, contributing to a deeper understanding of marine ecosystems and their response to environmental changes.

### Dataset features:

1. Salnty: Salinity (Practical Salinity Scale 1978) (outcome)
2. Depthm: cast depth in meters
3. O2mlL: Milliliters oxygen per liter of seawater
4. STheta: Potential Density (Sigma Theta), Kg/M3
5. O2Sat: Oxygen percent saturation
6. Oxyµmol/Kg: Oxygen micromoles per kilogram seawater
7. ChlorA: Migrograms Chlorophyll-a per liter seawater, measured fluorometrically
8. Phaeop: Micrograms Phaeopigment per liter seawater, measured fluormetrically
9. PO4uM: Micromoles Phosphate per liter of seawater
10. SiO3uM: Micromoles Silicate per liter of seawater
11. NO2uM: Micromoles Nitrite per liter of seawater
12. NH3uM: Micromoles Ammonia per liter of seawater
13. C14As1: 14C Assimilation of Replicate 1 (milligrams carbon per cubic meter of seawaterper half light day)
14. C14As2: 14C Assimilation of Replicate 2 (milligrams carbon per cubic meter of seawaterper half light day)
15. DarkAs: 14C Assimilation of Dark/Control Bottle (milligrams carbon per cubic meter ofseawater per half light day)
16. LightP: Light intensities of the incubation tubes in the primary productivity experiment,expressed as percentages
17. Year: The year the sample was collected

### Data Preprocessing:

- Handled missing values by dropping rows with missing salinity values and interpolating missing values for other features with linear interpolation.
- Normalized the data to scale the features to a similar range.
- Selected relevant features for predicting salinity, potentially dropping features with low Pearson correlation coefficients.

### Model:
Linear regression is a pivotal tool in the analysis of salinity dynamics in oceanic environments, particularly when combined with machine learning techniques. The salinity of seawater, a critical parameter influencing ocean circulation and ecosystem health, is often measured alongside various other oceanographic properties using instruments like Conductivity, Temperature, and Depth (CTD) casts.

In the context of the study utilizing the CalCOFI dataset, linear regression facilitates the exploration of relationships between salinity and a multitude of oceanographic features such as dissolved oxygen, chlorophyll-a, and nutrient concentrations. By employing linear regression models, researchers aim to understand how these variables interact with salinity and how they collectively influence marine ecosystems.


### Model Evaluation:

Evaluated the performance of the model using metrics such as 
- R^2
- Pearson’s correlation coefficient
- mean absolute error (MAE)

