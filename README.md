# E-Bike-Ownership-Model-NRW-GitHub

A paper associated with this code is currently under review. Once published, the publication will be added here and can be used to reference this code. A license will also be specified then.


Cells_elevar.ipynb

Python code which computes the elevar ("slope") attribute for 1km-Gridcells.

Uses the GeoGitter Inspire (https://gdz.bkg.bund.de/index.php/default/geographische-gitter-fur-deutschland-in-lambert-projektion-geogitter-inspire.html) and a dataset provided exclusively by Jan Kuchhäuser, Chair of Freight Transport Planning and Transport Logistics, University of Wuppertal.

Generates a csv-file with the elevar attribute for the grid cells as well as some figures.


Cells_spatial_type.ipynb 

Python code which writes one of four RegioStaR spatial types to 1km-grid cells.

Uses the output from cells_elevar, the GeoGitter Inspire (for 250m cells with municipality code) and the RegioStaR dataset (www.bmvi.de/regiostar).

Generates a csv-file with the spatial type attribute for the grid cells as well as some figures.


Data_processing_Ownership.ipynb

Python code which combines the B3 MiD person data with the elevar and spatial type data and processes it (clean data, create dummies, etc.).

Generates a csv-file with all person-level observations and the dependent and explanatory variables.


MiD_Ownership_Logit.ipynb

Python code using Biogeme (https://transp-or.epfl.ch/documents/technicalReports/Bier23.pdf) to estimate a multinomial Logit model.


MiD_Ownership_mvProbit R.ipynb

R code using mvProbit (https://cran.r-project.org/web/packages/mvProbit/index.html) to estimate a multivariate Probit model.
