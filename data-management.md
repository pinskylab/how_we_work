# Pinsky Lab Data Management Plan

The Pinsky Lab is an open science lab that believes in reproducible science.  To that aim:
1. We keep lab notebooks to record what we did, learned, or produced each day. Can be physical notebooks, text files, Evernote, Jupyter notebooks, etc.
1. We do our data analysis in GitHub repositories in the pinskylab organization to facilitate collaboration and sharing within the lab.
1. We keep our raw data in the github repository related to the project, unless the data files are too large.
    1. We generally use a folder called "data" within the repository.  
    1. We store our raw data with metadata describing what’s in the file and what the columns mean
    1. If we clean the data, we often use a folder called something like "data-raw" and a folder called "data-clean" to differentiate data in its original form from data that has been manipulated.
    1. If we are using data downloaded from another data source, we often have a folder called "data_dl" for downloaded data, that is not tracked in GitHub. We include the data source in a README file for reproducibility.
1. If our data are too large to store on github, please store them on the shared folder in Amarel (/projects/f_mlp195/) and/or the Pinsky Lab or (Restricted) Pinsky Lab folders on Box.
1. We back up our data in at least two places (beyond our computers). The cloud can be one site. An external harddrive can be another. Many lab members also choose to keep data copies on Amarel, Annotate, or another computing cluster. 
1. We use scripts to process data, make models, do analyses, etc.
1. We publish git repositories through Zenodo upon publication of a manuscript.
1. Collaborative manuscripts are written in google drive.
1. We generally make presentations in google slides so that other lab members can easily access useful graphics.
1. When matriculating, make sure all projects, code, papers, data, etc. are in the Pinsky Lab organization on GitHub or Google Drive.
