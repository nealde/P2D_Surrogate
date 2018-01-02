# P2D_Surrogate

### Neal Dawson-Elli, Seong Beom Lee, Manan Pathak, Kishalay Mitra, Venkat. R.  Subramanian

This repository will contain some of the code and models used in the paper **Data Science Approaches for Electrochemical Engineers – An Introduction through Surrogate Model Development for Lithium-Ion Batteries**
by the above authors.  The only required packages are `scikit-learn`,  `numpy`, and `matplotlib`, and an anaconda environment `requirements.txt` is supplied.

A `jupyter notebook` is supplied, as well as a python file that creates an image of the plot from matplotlib.

In order to run the supplied files, head over to [Anaconda](https://www.anaconda.com/download/?lang=en-us) and download the `Python 3.6` version of anaconda.

Once it is installed, open `Anaconda Prompt`, a special version of command prompt, and create a new environment using:

`conda create -n paper`

`activate paper`

A single-line installer is:
`conda install python=3.6 scipy=1.0.0 scikit-learn=0.19.1 matplotlib=2.1.1 jupyter`

Then, type: `jupyter notebook` and a jupyter notebook kernel will start.  Navigate to the repository folder in the jupyter file explorer and open `Recurrent_GBM.ipynb`.  The code should work.

To upload your own discharge data, simply swap out the CSV located in the targets folder.  It will attempt to fit any discharge data with less than 1800 seconds of discharge time, but it may only be accurate for discharge curves ending between 1400 and 1800 seconds, and is not garaunteed to be accurate at all.


