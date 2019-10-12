Dennis Zhao's copy of code for MOVEMENT DISORDER GAIT DATA Project

By Richard Sowers <r-sowers@illinois.edu>, website
<http://publish.illinois.edu/r-sowers/>
based on work led by
Manuel Hernandez <mhernand@illinois.edu>, website
http://kch.illinois.edu/hernandez


This is an analysis of MOVEMENT DISORDER GAIT DATA data.

* **Distance_difference_analysis_for_all_data.ipynb** 
   Calculate the distance between each step for L-L, L-R, R-L, R-R patterns from all available patient and health people data. Both patient and health people group will have four pairs of means and std nparray generated for each pattern. This file will be used further in Statistical_TwoSample_T_Test_Analysis.ipynb.
   
* **Statistical_TwoSample_T_Test_Analysis.ipynb** 
   Using data which are cleaned and generated in "Distance_difference_analysis_for_all_data.ipynb" to perform statistical tests. Shapiro–Wilk test and Levene’s test are used to check normality and homogenous. Then we performed two sample t test on each pair of patient mean and health mean for all four patterns. Boxplots, histogram, and normal Q-Q plot are included. 
   
* **Stride_MidSSL's_and_MidSSR's_x__y_vs_time.ipynb** 
   Using time interval of every second [i, i+1), we compare patients' (x, y) coordinates with healthy people's, and we applied a SVM at the end. 
   
* **Gait_data_speed_comparison.ipynb** 
   Cleaned data and tested patient's average stride speeds against health people's average stride speeds. We did various statistical test at the end. 
   
* **generate_new_data_before_training.ipynb**
    generate a new dataframe based on the features we found should be significant. Then run random forest to check each feature's importance.
