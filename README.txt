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
-
-
*****************************************************************************************************************************************
basic_feature_engineering_v3: Builds on basic_notebook2 and considers data from all the data sources: 
- train 
- test
- structures
- dipole_moments
- magnetic_shielding_tensors
- mulliken_charges
- potential_energy
- scalar_coupling_contributions

This book builds on previous notebooks regarding feature enginnering and feature selection however in this book we will train a model per coupling type.


*****************************************************************************************************************************************
basic_feature_engineering_v4: Builds on basic_notebook2 + basic_notebook3 and also only considers data from the following csv files: 
- train 
- test
- structures 

This book builds on previous notebooks regarding feature enginnering and feature selection however in this book we will train a model per coupling type.

*****************************************************************************************************************************************
basic_feature_engineering_v5: This book will try to develop an algorithm to identify an atoms nearby functional groups, that is, in CH3-CH2-OH the atoms
in CH3 are part of a CH3-group, neigherst neighbor are CH2 followed by OH. 
Only considers data from the following csv files: 
- train 
- test
- structures 

*****************************************************************************************************************************************
basic_feature_engineering_v6: This book will try to develop an algorithm to identify an atoms nearby functional groups, that is, in CH3-CH2-OH the atoms
in CH3 are part of a CH3-group, neigherst neighbor are CH2 followed by OH. In contrast to notebook 5 this one will be relying on Open Babel to find the 
SMILES of the molecules and use that to generate the fuctional groups present in the molecule

Only considers data from the following csv files: 
- train 
- test
- structures 
- xyz structure files
