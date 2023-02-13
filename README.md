# Nearby_Star_Catalog
This catalog contains 2575 stars within 20 parsecs from the Earth, mainly based on the Gaia Catalog of Nearby Stars (GCNS, see J/A+A/649/A6 on Vizier), with more completed parameters including stellar luminosity, effective temperature, radius, and mass. Following are descriptions for columns in the NSC & Habitable Zone results. 

# 1. Descriptions for NSC_20pc.csv

Num: Serial number of stars in the NSC, 1\~2575;\
type: I: Teff & G-band magnitude are known; II: only G-band magnitude is known; III: only Teff is known; IV: Teff & G-band magnitude are unknown;\
ra & dec: coordinates, mainly at Ep=2015.0/2016.0 (from Gaia DR2 & DR3);\
plx: parallax of stars, in mas;\
e_plx: error of parallax, in mas\;
GAIAmag: G-band magnitude;\
e_GAIAmag: error of G-band magnitude;\
pmRA: proper motion in RA direction;\
pmDEC: proper motion in DEC direction;\
e_pmRA: error in proper motion in RA direction;\
e_pmDEC: error in proper motion in DEC direction;\
MASS&massSrc: stellar mass (in Msun) of the star and the source of it;\
RAD&radSrc: stellar radius (in Rsun) of the star and the source of it;\
TEFF&TeffSrc: stellar effective temperature (in Kelvin) of the star and the source of it;\
MH&mhSrc: stellar metallicity (M[H]) of the star and the source of it;\
LOGG&loggSrc: surface gravity (in log scale) of the star and the source of it;\
lum: stellar luminosity (in Lsun) of the star;\
e_lum: error in stellar luminosity (in Lsun) of the star;\
Tmag: T-band magnitude, from TIC catalog;\
e_Tmag: error in Tmag;\
Bmag~e_w4mag: magnitudes in various bands. Note that 'gmag' in these columns are not Gaia magnitudes;\
d: distance of the star (from TIC)\
e_d: error in distance\
eneg_Mass: negative error in mass;\
epos_Mass: positive error in mass;\
eneg_Rad: negative error in radius;\
epos_Rad: positive error in radius;\
eneg_logg: negative error in surface gravity (in log_10 scale);\
epos_logg: positive error in surface gravity (in log_10 scale);\
eneg_lum: negative error in luminosity;\
epos_lum: positive error in luminosity;\
eneg_Teff: negative error in effective temperature;\
epos_Teff: positive error in effective temperature;\
gaiabp: Gaia Bp magnitude;\
e_gaiabp: error in Gaia Bp magnitude;\
gaiarp: Gaia Rp magnitude;\
e_gaiarp: error in Gaia Rp magnitude;\
\_RAJ2000: right ascension, in J2000.0, sexa;\
\_DEJ2000: declination, in J2000.0, sexa;\
FG: G-band mean flux;\
e_FG: error in G-band mean flux;\
FBP: mean flux in the integrated Bp band;\
e_FBP: error in the mean flux in the integrated Bp band;\
FRP: mean flux in the integrated Rp band;\
e_FRP: error in the mean flux in the integrated Rp band;\
BP-RP: BP-RP colour;\
RV: Spectroscopic radial velocity in the solar barycentric reference frame;\
e_RV: error in radial velocity;\
PM: total proper motion of the star;\
RAJ2000: right ascension, in J2000.0, in deg;\
DEJ2000: declination, in J2000.0, in deg;\
AG: Estimate of extinction in the G band from Apsis-Priam; (for details of Apsis-Priam: see https://arxiv.org/pdf/1804.09365.pdf) \
E(BP-RP): Estimate of redenning E(BP-RP) from Apsis-Priam;\
B-V: the B-V colour index;\
PS1: object identifier of the Pan-STARRS release 1 (PS1) Survey - DR1;\
SDSSDR13: object identifier the SDSS Photometric Catalogue, Release 13;\
SkyMapper2: object identifier of SkyMapper-2;\
URAT1: object identifier of uric acid transporter 1;\
TIC: object identifier of the TESS Input Catalog;\
HIP: object identifier of the Hipparcos Catalog;\
TYC: object identifier of the Tycho Catalog;\
UCAC: object identifier of the USNO CCD Astrograph Catalog;\
TWOMASS: object identifier of TWOMASS;\
SDSS: object identifier of the Sloan Digital Sky Survey;\
ALLWISE: object identifier of ALLWISE;\
APASS: object identifier of the AAVSO Photometric All-Sky Survey;\
KIC: object identifier of the Kepler Input Catalog.

# 2. Descriptions for Habitable_Zone_Results.csv

dis: distance (pc);\
teff: effective temperature (K);\
lum: luminosity (Lsun);\
mass: mass (Msun);\
rad: radius (Rsun);

mas_IHZ: inner bound of habitable zone(mas);\
mas_OHZ: outer bound of habitable zone(mas);\
AU_IHZ: inner bound of HZ(AU);\
AU_OHZ: outer bound of HZ(AU);\
TRp_IHZ: transit rate for planets at inner bound of HZ;\
TRp_OHZ: transit rate for planets at outer bound of HZ;\
TRt_IHZ: transit duration for planets at inner bound of HZ(hour);\
TRt_OHZ: transit duration for planets at outer bound of HZ(hour);\
TRD: transit depth;\
Ast_max_IHZ: maximum stellar amplitude for planets at inner bound of HZ(μas);\
Ast_max_OHZ: maximum stellar amplitude for planets at outer bound of HZ(μas);\
RV_max_IHZ: maximum stellar radial velocity for planets at inner bound of HZ(m/s);\
RV_max_OHZ: maximum stellar radial velocity for planets at outer bound of HZ(m/s);\
RV_E_IHZ: stellar radial velocity expectation (<sin i>=pi/4) for planets at inner bound of HZ(m/s);\
RV_E_OHZ: stellar radial velocity expectation (<sin i>=pi/4) for planets at outer bound of HZ(m/s);\
BR_IR_IHZ: blackbody radiation ratio of planet to star for planets at inner bound of HZ @10μm band;\
BR_IR_OHZ: blackbody radiation ratio of planet to star for planets at outer bound of HZ @10μm band;\
RR_IHZ:: radiation ratio of planet to star for planets at inner bound of HZ;\
RR_OHZ: ratio of planet to star for planets at outer bound of HZ;\
MDTV_IHZ: the aperture diameter requirements for planets at inner bound of HZ @550nm(m);\
MDTV_OHZ: the aperture diameter requirements for planets at inner bound of HZ @550nm(m);\
MDTIR_IHZ: the aperture diameter requirements for planets at inner bound of HZ @10μm(m);\
MDTIR_OHZ: the aperture diameter requirements for planets at outer bound of HZ @10μm(m);

Following parameters are for planets at the center of HZ:	

Detect_TR: detect possibility via transit method(Transit depth＞30ppm @Vmag=7);\
Detect_RV: detect possibility via RV method(stellar radial velocity >0.2m/s @Vmag=8);

500nm: radiation ratio of planet to star@500nm band;\
4000nm: radiation ratio of planet to star@4000nm band;\
7500nm: radiation ratio of planet to star@7500nm band;\
11000nm:	radiation ratio of planet to star@11000nm band;\
tmag: TESS magnitude;\
RVE: stellar radial velocity expectation(m/s).

