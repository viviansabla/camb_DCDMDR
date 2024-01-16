CAMB_DCDMDR
-----------

Authors: Vivian Sabla

This is a modified version of the Einstein-Boltzmann code CAMB, modified to include a CDM->DR component.
Original code can be found at https://github.com/cmbant/CAMB. This code is modified from the August 2018
version of CAMB.
Background dynamics specified simply by:

$\rho_{dcdm}'+3\mathcal{H}\rho_{dcdm} =-a\Gamma_{dcdm}  \rho_{dcdm}$

$\rho_{dr}'+4\mathcal{H}\rho_{dr} =a\Gamma_{dcdm}  \rho_{dcdm}$. 

Perturbations for the dark radiation (dr) follow a full Boltzmann hierarchy. 
$\Gamma_{dcdm}$ represents the decay constant and is defined in units of 1/Gyr.

All modifications from original CAMB are labelled with a comment consisting of my initials 'VS' followed by the date of modification.

Compilation and Usage
---------------------
To install the code, do:
  cd camb_DCDMDR
  make clean
  make
To check that it compiled correctly, do:
  ./camb paramsDCDM.ini

In the .ini file, the density of the decaying component of CDM is set via omc2h2, and the dark radiaiton component is omdrh2. 
The decay constant is set via gamma_dcdm. 

Support
-------
If you have questions or problems, please email vivian.iossa.sabla@gmail.com
