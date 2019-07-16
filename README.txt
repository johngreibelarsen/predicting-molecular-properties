basic_notebook: Serves to load the data and get a understanding for it. This book will only consider data from the following csv files: 
- train 
- test
- structures 

No feature enginnering or selection are performed and no model tuning.
score 1.1405594098789402
ranking: top 85%

*****************************************************************************************************************************************

basic_feature_engineering_v1: Builds on basic_notebook and also only considers data from the following csv files: 
- train 
- test
- structures 

Feature enginnering and feature selection are performed, that said, this attempts to do the simplest physical model by calculating the radial distance 
between atomes and the 'no of bonds' distance leaving out cartesion coordinates and other features considered 'noisy'. No model tuning is performed.
HOWEVER IT DOES NOT LOOK LIKE IT IS WORKING AND I DON'T UNDERSTAND WHY - in particular it works for split training and validation data but not on the 
test data!!

Next version will leave all 'noisy data' in the data set
*****************************************************************************************************************************************
