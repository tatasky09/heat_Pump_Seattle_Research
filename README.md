## A Scalable Data-Driven Method for Mapping Building Electrification: Hybrid Rule-Based and Machine Learning Classification of Heat-Pump Adoption

As U.S. cities pursue ambitious decarbonization goals, electrifying space heating and cooling has become a key strategy. Medium to large multifamily buildings are central to this transition, and Seattle has prioritized this sector in its path toward net-zero emissions. However, administrative trade permit data—often incomplete and inconsistently reported—creates challenges for analyzing heat pump adoption and informing policy decisions.
This study presents a two-stage hybrid methodology to classify multifamily building permits by heat pump installation scope. The first stage applies HVAC-informed rules using numeric indicators such as chiller capacity to floor area ratio, tonnage per dwelling unit, and compressor density. Thresholds are tailored to building typologies (low-, mid-, and high-rise) to infer system coverage. Systems meeting ≥80% of expected load are labeled as Whole Building, while lower ratios suggest Common Areas Only. Text-based cues (e.g., “lobby,” “retail,” “single zone”) and unit-ratio checks further refine classification, producing a labeled dataset and an “uncertain” pool.
The second stage employs a supervised model to classify uncertain cases. Text fields are embedded using a sentence-transformer and fused with standardized numeric features. A machine learning model is trained on rule-labeled data, validated via stratified cross-validation, and enhanced through semi-supervised pseudo-labeling at a confidence threshold of 0.85.
Preliminary regression analysis shows that buildings with whole-building heat pump installations command significantly higher rents than those with partial or no systems. This interpretable and scalable framework improves classification accuracy for messy permit records, supporting data-driven electrification policy and encouraging broader adoption of heat pumps in multifamily housing.


Figure 1: Total Class A and Class B Apartment Buildings with and without Heat Pump

<img src="images/media/image1.png" alt="Graph showing apartment buildings with and without heat pumps" width="800" />

Figure 2: Average Asking Rent Over Time by Heat Pump Status

<img src="images/media/image2.png" alt="Graph of average asking rent over time" width="800" />

Figure 3: Median Asking Rent Over Time by Heat Pump Status

<img src="images/media/image3.png" alt="Graph of median asking rent over time" width="800" />

Figure 4: Heat Map of Apartment Buildings with Heat Pump Installed

<img src="images/media/image4.png" alt="Heat map of apartment buildings with heat pumps installed" width="800" />

Figure 5: Heat Pump Installation Ratio by Census Tract

<img src="images/media/image5.png" alt="Map showing heat pump installation ratio by census tract" width="800" />

Figure 6: Asking Rent Over Time by Heat Pump Status and Building Classes

<img src="images/media/image6.png" alt="Graph of asking rent over time by heat pump status and building classes" width="800" />

Figure 7: Heat Pump Coverage Status Over Time (Classified Using Semi-Supervised Machine Learning Technique)

<img src="images/media/image7.png" alt="Graph showing heat pump coverage status over time using machine learning" width="800" />

Figure 8: Average Effective Rent by Heat Pump Coverage Status Over Time (Classified Using Semi-Supervised Machine Learning Technique)

<img src="images/media/image8.png" alt="Graph of average effective rent by heat pump coverage status" width="800" />

