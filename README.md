# REGRESIONDISCONTINUA
CODIGO REGRESION DISCONTINUA
ESTIMACION DE REGRESION DISCONTINUA DIFUSA
rdrobust trabajo18 rnv_h if group==1, h(6) b(11) fuzzy(bdh_2) kernel(triangular) vce(nncluster ?
certificado2014) all
Estimaciones horas
eststo i1: rdrobust horas rnv_h if group==1, h(6) b(11) fuzzy(bdh_2) kernel(triangular) ?
vce(nncluster certificado2014) all
?*****************************************************************************?
?*Mccrary Test base 2014?
?*****************************************************************************?
?*1. Generamos nucleos del hogar?
egen id_nucleo = concat (certificado idnucleo), format(%20.0g)?
?*Test?
rddensity rnv, plot
?*Rnv= running variable centrado al corte?
