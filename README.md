# FluPRINT
Code for applying Stabl &amp; MoFA to FluPRINT dataset.

## MOFA
MOFA requires renaming of data to fit terminology. Donor ID is renamed to sample, data name to feature, assay to view, and data to value. Additionally, since MOFA does not take outcome into account during its analysis, outcome must be represented as a part of metadata, called group. 

Other metadata columns such as age, BMI, gender, and race do not need to be kept in the final input data for MOFA as it will not utilize them for their factor analysis. However, any of these properties can be converted to a discrete variable and put as group instead of outcome. 

## Stabl
Stabl does not require specific terminology. Renaming of columns was done to be consistent with MOFA analysis. Metadata was dropped for Stabl analysis, but each can be kept as another feature. 
