A paper associated with this code is currently under review. Once published, the publication will be added here and can be used to reference this code.


01_cells spatial typology.ipynb 

Python code which writes one of four RegioStaR spatial typologies to 1km-grid cells.

Uses the GeoGitter Inspire (for 250m cells with municipality code) and the RegioStaR dataset (www.bmvi.de/regiostar).

Generates a csv-file with the spatial type attribute for the grid cells as well as some figures.


02_cells gradient.ipynb

Python code which computes the gradient attribute for 1km-Gridcells.

Uses the GeoGitter Inspire (https://gdz.bkg.bund.de/index.php/default/geographische-gitter-fur-deutschland-in-lambert-projektion-geogitter-inspire.html), a dataset provided exclusively by Burgdorf M, Pütz T. Dokumentation der Raumvariablen des BBSR im Regionalfile. Annex 5 to the user manual for the MiD 2017. 2019., and the list of target grid cells created by 01_Cells spatial typology. 

Generates a csv-file with the gradient attribute for the grid cells.


10_Data processing.ipynb

Python code which combines the B3 MiD person data with the gradient and spatial typology data and processes it (clean data, create dummies, etc.).

Generates a csv-file with all person-level observations and the dependent and explanatory variables.


21_nested Logit.ipynb

Python code using Biogeme (https://transp-or.epfl.ch/documents/technicalReports/Bier23.pdf) to estimate a nested Logit model.


22_mv Probit.ipynb

R code using mvProbit (https://cran.r-project.org/web/packages/mvProbit/index.html) to estimate a multivariate Probit model.
