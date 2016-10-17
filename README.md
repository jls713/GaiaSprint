# Gaia Sprint Preparation

There are four notebooks with useful stuff in preparation for the Gaia Sprint.

1. [Distances](TGAS\ +\ Spectrophotometric\ Distances.ipynb) -- for the four spectroscopic surveys with large-ish overlap with TGAS (RAVE, APOGEE, GALAH, LEGUE) I have computed the distances by folding the spectrophotometric distances with the TGAS parallax estimate.

2. [Actions](TGAS\ actions.ipynb) -- for the same four surveys, I have computed the median actions, angles and frequencies for each stars along with their standard deviation y sampling from the covariant error ellipse (only using stars with $\delta\varpi/\varpi<0.2$ so use uniform prior).

3. [TGAS+RAVE](TGAS-RAVE.ipynb) -- sample from the Sanders & Binney EDF using the joint TGAS+RAVE selection function expressed in the J-band.

4. [TGAS+APOGEE](TGAS-APOGEE.ipynb) --  sample from Sanders & Binney EDF using the plate-by-plate APOGEE selection function (i.e. uniform in H between limits obtained from Bovy code). The TGAS+APOGEE selection function is then estimated by dividing the TGAS+APOGEE sample by APOGEE in the H-band and applied to the mocks. This doesn't work so well as the selection function obviously haas significant color dependence from TGAS.

All the distance files used can be found [here](www.ast.cam.ac.uk/~jls/distances/).

All the action files used can be found [here](www.ast.cam.ac.uk/~jls/actions/).

All the EDF sample files used can be found [here](www.ast.cam.ac.uk/~jls/edf/).
