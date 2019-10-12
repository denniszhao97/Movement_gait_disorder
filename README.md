Dennis Zhao's copy of code for MOVEMENT DISORDER GAIT DATA Project

By Richard Sowers <r-sowers@illinois.edu>, website
<http://publish.illinois.edu/r-sowers/>
based on work led by
Manuel Hernandez <mhernand@illinois.edu>, website
http://kch.illinois.edu/hernandez


This is an analysis of MOVEMENT DISORDER GAIT DATA data.

* **Distance_difference_analysis_for_all_data.ipynb** 
   Calculate the distance between each step for L-L, L-R, R-L, R-R patterns from all available patient and health people data. Both patient and health people group will have four pairs of means and std nparray generated for each pattern. 
* **Statistical_TwoSample_T_Test_Analysis.ipynb** 
   Using data which are cleaned and generated in "Distance_difference_analysis_for_all_data.ipynb" to perform statistical tests. Shapiro–Wilk test and Levene’s test are used to check normality and homogenous. Then we performed two sample t test on each pair of patient mean and health mean for all four patterns. Boxplots, histogram, and normal Q-Q plot are included. 
* **Stride_MidSSL's_and_MidSSR's_x__y_vs_time.ipynb** 
   Using fixed time interval from 30s-60s, we compare patients' (x, y) coordinates with healthy people's 
* **Gait_data_speed_comparison.ipynb** 
   Cleaned data and tested patient's average stride speeds against health people's average stride speeds.  
* **Matched_Timing_of_Force_and_Mid_Stances.ipynb**
    Matched eventimes in RAWDATA and GAITCYCLES, identified x coordinate of Mid stances as a significant explanatory variable.
* **Centroid for Strides.ipynb**
    Data Visualization of patient 200's and 300's trial 1 and trial 2 stride patterns over time. 
* **vertical_acc_mean_std.ipynb**
    Comparision between the healthy people's and the patients' vertical accelerations.
* **light_and_heavy_step.ipynb**
    Calculate light, heavy, and normal steps.
* **generate_new_data_before_training.ipynb**
    generate a new dataframe based on the features we found should be significant. Then run random forest to check each feature's importance.
