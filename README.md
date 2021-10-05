# RecoderPlus
A program for pre-processing background data and prepare it for conditioning

About RecoderPlus

RecoderPlus is an SPSS macro that reads in a set of variables from an SPSS system file, and processes them in one of 3 ways:

1.	Creates contrast coded variables for the variables listed as CATVARS. Contrast coding can be done using dummy or effect coding by using the parameter CONTYPE.

2.	Imputes missing values for a variable with the mean of the non-missing values for variables      listed as IMPMEAN. It can impute using the overall mean across all cases, or within groups defined by the variables BYVARS. It also creates a dummy coded variable indicating those cases with missing values in the original variable, which values were imputed.

3.	Recodes the values of the variable listed as USECRIT to the mean for the group on the criterion variable CRITVAR. The imputed value could be calculated across the entire sample, or within the group defined by the variables BYVARS.
In addition to recoding individual variables, it creates interaction variables between pairs of original variables, using the recoded vectors.

Requirements

RecoderPlus requires a working copy of SPSS installed in the computer where the analysis is conducted. It also requires an SPSS system file with at least one variable to be recoded. When creating interaction variable, you will need at least 2 variables. Variables can be numeric of string variables.
