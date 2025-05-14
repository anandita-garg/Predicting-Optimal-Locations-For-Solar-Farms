# Predicting-Optimal-Locations-For-Solar-Farms

Importance of clean and renewable energy has been highlighted in recent years owing to
growing populations, over-consumption of natural resources, depletion of existing sources of
energy and rising concerns around global climate change. A shift to reliance on solar energy
has emerged as a viable alternative to fossil fuels. In India, solar energy has significantly
contributed to the renewable energy sector in recent years, accounting for 92.12 GW out of
the 203.18 GW of clean energy generated. Therefore, identifying ways of maximizing the
potential of solar energy remains an area requiring extensive research.

The deployment of solar farms is a key aspect of this effort, driving studies aimed at
predicting and selecting optimal sites for photovoltaic farm installations. Factors such as
terrain data, geographic location, environmental elements like temperature, wind speed and
precipitation, are often considered important.

A review of past studies has revealed that methodologies primarily employ statistical
methods. These models are based on subjective Multi-Criteria Decision-Making (MCDM)
techniques, such as the Analytic Hierarchy Process (AHP) and Weighted Linear Combination
(WLC). Studies that use artificial intelligence and machine learning are significantly less
relevant and developed in the current state of the domain, especially in the Indian
context.

Here, we present a model that is driven by an AI-ML approach to predict optimality of
locations for installation of solar farms. Our approach would enable highly precise assessments
of potential solar farm locations, taking into account a multitude of factors such as temperature,
wind speed, precipitation, sunshine duration, and terrain analysis through data from tools
such as Google Earth Engine and segmentation of satellite images. We expect our study to
contribute significantly towards efforts to achieve and improve energy efficiency, cost savings,
and sustainability with regards to solar power. This approach would aim to enhance return on
investment and encourage more widespread adoption of solar energy solutions.

Our methodology involved acquiring geographical data from sources such as OpenMeteo and Google Earth
Engine. The features considered were based on our literature study; features which were deemed most
significant for picking locations for solar farm installations. Some of these features corresponded to
those in papers that employed AHP-based models. We referred to the features matrices in two of such papers to 
calculate the ground truth values while additional features were used for training our ML model alongside the
AHP highlighted features. 

After splitting our dataset based on temporal analysis (taking specific solar farm coordinates for training
and test set based on their year of commission), we used the following ML algorithms to train our model : Random Forest,
K-Nearest Neighbours, Support Vector Machines, Multi-Layer Perceptron and XGBoost. XGBoost turned out as the best 
performing model with a Mean Squared Error of 0.0135 and an R² values of 0.7915. Further, we validated our model. We also implemented SHAP for interpretability.
