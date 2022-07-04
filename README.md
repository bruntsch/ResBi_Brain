# ResBi_Brain
Code of my master thesis investigating functional connectivity changes within the fronto-limbic network and default mode network of participants with bipolar disorder or being at-risk of developing it and healthy controls. Code contains resting-state analysis with nilearn, statistical analysis and plots of the results.

The analysis steps are ordered from 1 to 4: 
  1. Creating a mask for all ROIs (containing regions of the FLN and DMN) based on the DiFuMo atlas
  2. Extracting of the timeseries of every participant and calculation the partialy correlation matrices based on the individual timeseries for each subject + calculating the group partial correlation matrices
  3. Creating a dataframe that contains all the necessary information (demographical data + partial correlation values of all connections for each participant)
  4. Calculating an OLS regression for the effect of the groups and IDSC & YMRS scores
  
Further, the code for every visualisation is made available, containing: 
 - connectome and circular plots for the groups 
 - plot of all the regions contained within the created mask
 - plot of a single-subject partial correlation matrix
