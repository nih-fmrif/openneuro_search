# OpenNeuro Search

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nih-fmrif/openneuro_search/HEAD?labpath=notebooks%2Fopenneuro_search.ipynb)


The search functionality on OpenNeuro is pretty good and it's getting better, but sometimes you want to search based on specific image parameters. In this case, I wanted to find all of the datasets that had at least 2 runs of resting state date with resolution of 2x2x2 or better. I first cloned `///openneuro` with datalad to the data directory here, then used the code in `notebooks/openneuro_search.ipynb` to find the first bold sequence from each dataset, `get` it with datalad, and pull the dimension information from the header with `nilearn.image`. 