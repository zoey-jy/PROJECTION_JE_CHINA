Software dependencies
For the development of the code in this repository we made use of the following R packages (in a macOS environment):

data.table version 1.14.0
tidyverse version 1.3.1
lubridate version 1.7.10
ModelMetrics version 1.2.2.2
rgdal version 1.5-23
magrittr version 2.0.1
mgcv version 1.8-35
readr version 1.4.0
spdep version 1.1-11
reshape2 version 1.4.4
There is no need for non-standard hardware.
# DATA
Japanese encephalitis surveillance data are available at the National Notifiable Disease Surveillance System of the Chinese Center for Disease Control and Prevention (China CDC). To access these data and/or to seek permission for its use, please contact the Data-center of China Public Health Science (https://www.phsciencedata.cn/Share/index.jsp) or email data@chinacdc.cn. Mosquito vector density data is subject to restrictions for the protection of privacy. Requests for data access should be addressed to the corresponding authors. Historical meteorological data was obtained from the China Meteorological Data Sharing System (http://data.cma.cn/). CMIP6 data are available at https://esgf-ui.ceda.ac.uk/ cog/search/cmip6-ceda/. All other data utilized in this study were accessed from open sources. 
#Expected output
After running all files you should get the following output

00_blocked_cross_validation.R: Generates a suite of .csv files named metric_equation_x_block_y.csv where metric indicates the name of the metric used (i.e., MAE, BIC, AIC, Spearman correlation), x indicates the equation being investigated, and y the cross-validation block. Estimated running time: 3 days using a High Performance Computer if you want to run all possible combinations of covariates.
