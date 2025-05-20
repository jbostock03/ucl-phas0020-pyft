# Final Python Task: Didymos Investigation

Python Final Task for PHAS0020 at University College London

## Files
In `./files` are the `.fits` files used for the investigation, as well as the Notebook with all calculations: `pyft.ipynb`.

## Introduction
The main focus of this notebook is an investigation into the asteroid of Didymos. The magnitude of the Didymos system was calculated to be $12.92 \pm 0.08$, which is in agreement with the calculated value by A. Graykowski et al. of $m_v = 12.96 \pm 0.04$, for a similar time of observation, once the fast-moving ejecta was no longer in the aperture.

To obtain this magnitude, I first performed aperture photometry ab initio on 10 reference stars chosen arbitrarily in one of the provided frames, to be able to linearly calibrate magnitude and counts. The process of aperture photometry was then rerun on three more frames, in order to compile a mean flux trend curve over time. This allowed for detrending of the fluxes obtained from aperture photometry. Using this trend, it was possible to calculate a mean flux for Didymos to use in the earlier linear calibration to lead to an interpolated magnitude of Didymos.

In addition to aperture photometry, the angular velocity of Didymos was calculated as $0.105 \pm 1.411 \degree$ /hr. The recorded value from the JPL Ephemeris service is $0.107 \degree$ /hr, which is a 2% difference to the calculated value. This was achieved by doing linear fits to both RA and Dec.

Finally, I investigated briefly the trail from Dimorphos -- a smaller asteroid in orbit around Didymos -- of which the trail was caused by NASA's DART mission. I conducted aperture photometry using an elliptical aperture, which led to a calculation of flux of $140 \pm 30$ ADUs/arcsec.
