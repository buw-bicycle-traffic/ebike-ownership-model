A paper associated with this code is currently under review. Once published, the publication will be added here and can be used to reference this code. A license will also be specified then.


01_Cells_elevar.ipynb

Python code which computes the gradient ("elevar") attribute for 1km-Gridcells.

Uses the GeoGitter Inspire (https://gdz.bkg.bund.de/index.php/default/geographische-gitter-fur-deutschland-in-lambert-projektion-geogitter-inspire.html) and a dataset provided exclusively by Jan Kuchhäuser, Chair of Freight Transport Planning and Transport Logistics, University of Wuppertal.

Generates a csv-file with the gradient attribute for the grid cells as well as some figures.


02_Cells spatial typology.ipynb 

Python code which writes one of four RegioStaR spatial typologies to 1km-grid cells.

Uses the output from "01_cells gradient", the GeoGitter Inspire (for 250m cells with municipality code) and the RegioStaR dataset (www.bmvi.de/regiostar).

Generates a csv-file with the spatial type attribute for the grid cells as well as some figures.


10_Data processing.ipynb

Python code which combines the B3 MiD person data with the gradient and spatial typology data and processes it (clean data, create dummies, etc.).

Generates a csv-file with all person-level observations and the dependent and explanatory variables.


21_mn Logit.ipynb

Python code using Biogeme (https://transp-or.epfl.ch/documents/technicalReports/Bier23.pdf) to estimate a multinomial Logit model.


22_mv Probit.ipynb

R code using mvProbit (https://cran.r-project.org/web/packages/mvProbit/index.html) to estimate a multivariate Probit model.
