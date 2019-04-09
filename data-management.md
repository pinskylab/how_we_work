# Pinsky Lab Data Management Plan

The Pinsky Lab is an open science lab that believes in reproducible science.  To that aim:
1. We do our data analysis in GitHub repositories in the pinskylab organization to facilitate collaboration and sharing within the lab.
1. We keep our original data in the github repository related to the project, unless the data files are too large.
    1. We generally use a folder called "data" within the repository.  
    1. If you clean the data, you might want a folder called something like "data-raw" and a folder called "data-clean" to differentiate data in its original form from data that has been manipulated.
    1. If you are using data downloaded from another data source, you might want to have a folder called "data_dl" for downloaded data, that is not tracked in GitHub. But make sure to include the source in a README file for reproducibility.
1. If our data are too large to store on github, please store them on the lab server in /local/shared/pinskylab/.
1. We publish git repositories through Zenodo upon publication of a manuscript.
1. Collaborative manuscripts are written in google drive.
1. We generally make presentations in google slides so that other lab members can easily access useful graphics.
1. When matriculating, make sure all projects, code, papers, data, etc. are in the Pinsky Lab organization on GitHub or Google Drive.
