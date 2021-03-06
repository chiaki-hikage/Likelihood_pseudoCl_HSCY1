# Contents
This is the likelihood codes of HSC Y1 cosmic shear power spectrum and relevant data,
which used in C. Hikage, PASJ 71 (2019) 43 (arXiv:1809.09148)

The likelihood is available in the Monte Python (The Monte Carlo code for CLASS in Python)
and download it from the following:
 https://baudren.github.io/montepython.html

1. Add the HSC pseudo-Cl likelihood "HSC_Y1_pseudoCl_likelihood" into montepython/likelihoods/

2. Set the montepython directryname (dir_montepython) in the file of prepare.sh
   You can also change various parameters such as samplers and the parameters

3. Run the shell script prepare.sh, which makes the input files to run the code

4. Run the likelihood code as
   sh jobscript.sh (or qsub jobscript.sh to submit the job in clusters)


This code work with Python 2.7.5 and the library used in this code is
 Numpy, Scipy, 
 Monte Python 2.2.2/3.0.1 (B. Audren), 
 MultiNest: v3.10/v3.11 (Feroz, Hobson) (if you want to run nestcheck, v3.11 is required),
 CLASS 2.6.3,
 CLASS with HMcode (Brieden, Archidiacono, Lesgourgues),
 Colossus 1.2.1 (Diemer 2018)


# References
Cosmology from cosmic shear power spectra with Subaru Hyper Suprime-Cam first-year data  
Chiaki Hikage, Masamune Oguri, Takashi Hamana, et al.  
Publ. Astron. Soc. Japan, Vol.71, Issue 2, 43 (2019)
