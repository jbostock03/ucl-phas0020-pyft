# Final Python Task: Didymos Investigation

Python Final Task for PHAS0020 at University College London

## Contents
- [Getting Started](https://github.com/jbostock03/ucl-phas0020-pyft#Getting-Started)
- [Introduction](https://github.com/jbostock03/ucl-phas0020-pyft#Introduction)
- [Author](https://github.com/jbostock03/ucl-phas0020-pyft#Author)
- [Acknowledgements](https://github.com/jbostock03/ucl-phas0020-pyft#Acknowledgements)

## Getting Started
In `./files` are the `.fits` files used for the investigation, as well as the Notebook with all calculations: `0pyft.ipynb`.

The project is viewable natively in GitHub simply through opening the Jupyter Notebook.

## Introduction
The main focus of this notebook is an investigation into the asteroid of Didymos. The magnitude of the Didymos system was calculated to be $12.92 \pm 0.08$, which is in agreement with the calculated value by A. Graykowski et al. of $m_v = 12.96 \pm 0.04$, for a similar time of observation, once the fast-moving ejecta was no longer in the aperture.

To obtain this magnitude, I first performed aperture photometry ab initio on 10 reference stars chosen arbitrarily in one of the provided frames, to be able to linearly calibrate magnitude and counts. The process of aperture photometry was then rerun on three more frames, in order to compile a mean flux trend curve over time. This allowed for detrending of the fluxes obtained from aperture photometry. Using this trend, it was possible to calculate a mean flux for Didymos to use in the earlier linear calibration to lead to an interpolated magnitude of Didymos.

In addition to aperture photometry, the angular velocity of Didymos was calculated as $0.105 \pm 1.411 \degree$ /hr. The recorded value from the JPL Ephemeris service is $0.107 \degree$ /hr, which is a 2% difference to the calculated value. This was achieved by doing linear fits to both RA and Dec.

Finally, I investigated briefly the trail from Dimorphos $\textendash$ a smaller asteroid in orbit around Didymos $\textendash$ of which the trail was caused by NASA's DART mission. I conducted aperture photometry using an elliptical aperture, which led to a calculation of flux of $140 \pm 30$ ADUs/arcsec.

## Author
[Josh Bostock](https://github.com/jbostock03)

This project was created as the _Python Final Task_ for the module _PHAS0020: Practical Astrophysics & Computing_ at University College London (February $\textendash$ March 2024).

## Acknowledgements
[1] [Light curves and colours of the ejecta from Dimorphos after the DART impact", Graykowski, A. et al. (2023)](https://www.nature.com/articles/s41586-023-05852-9) (accessed 3 Mar 2024)

[2] [JPL Ephemeris service](https://ssd.jpl.nasa.gov/horizons/app.html#/) (accessed 27 Feb 2024)

[3] ["Median" on Wikipedia](https://en.wikipedia.org/wiki/Median#Efficiency) (accessed 28 Feb 2024)

[4] "PHAS0020 pre-sessions basics revision (C)", Fossey, S. et al. (revised ver. 2023). Available from the PHAS0020 Moodle page under 'First half of Term 2: Computing with Python' as 'PHAS0020-S0c-JupyterN_PHAS0003-refresh.ipynb'. (accessed 21 Feb 2024)

[5] [AladinLite](https://aladin.cds.unistra.fr/AladinLite/) (accessed 27 Feb 2024)

[6] "Fitting a Function to Data", Waugh, B. (2022). Available from the PHAS0007 Experimental Physics Moodle page as 'FittingAFunctionToData(14.11.2022).ipynb'. (accessed 21 Feb 2024)

[7] "Data Analysis and Statistics Booklet", Szumilo, M. et al. (2022). Available from the PHAS0020 Moodle page under 'Data Analysis Lectures and Problem Sheet' as 'Data Analysis and Statistics Booklet (Yr1) (2022 update)'. (accessed 2 Mar 2024)

[8] ["Proper Motion" on Wikipedia](https://en.wikipedia.org/wiki/Proper_motion) (accessed 29 Feb 2024)

[9] ["65803 Didymos" on Wikipedia](https://en.wikipedia.org/wiki/65803_Didymos) (accessed 3 Mar 2024)

[10] ["Dimorphos Orbit Determination from Mutual Events Photometry", Scheirich, P. et al. (2024)](https://iopscience.iop.org/article/10.3847/PSJ/ad12cf) (accessed 3 Mar 2024)

[11] ["CHI-1, 60CM F6.5 REFLECTOR" on Telescope Live, under "CCD Camera Specification (CHI-1-CCD, discontinued in Jan 2023)](https://help.telescope.live/hc/en-us/articles/360002557197-CHI-1-60cm-F6-5-Reflector) (accessed 2 Mar 2024)

[12] ["NASA’s DART Mission Hits Asteroid in First-Ever Planetary Defense Test" (2022)](https://www.nasa.gov/news-release/nasas-dart-mission-hits-asteroid-in-first-ever-planetary-defense-test/) (accessed 3 Mar 2024)

[13] ["Ellipse" on Wikipedia](https://en.wikipedia.org/wiki/Ellipse) (accessed 3 Mar 2024)
