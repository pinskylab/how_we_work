# Pinsky Lab Data Management Plan

The Pinsky Lab perpetuates an open science policy to ensure accessible and reproducible science. To assist in achieving that aim:

##General project documentation
-------------------------------

1. Lab notebooks are maintained each day; tracking progress, daily learnings, what was accomplished, and/or what goal was worked towards. These can be physical notebooks, text files, Evernote, Jupyter notebooks, etc.
	a. It is asked that the lab notebook is digitally backed up, in the event of a worse-case scenario

2. GitHub repositories are utilized for storage of project componenents
	a. This facilitates of collaboration and sharing within the labs space

3. Raw data is stored in the GitHub repository associated with the project, when applicable
	a. Typically raw data can be found in a folder titled "data" in the assocated repository
	b. Metadata, a descriptor of the raw dataset, is stored with with the raw data
	c. If data is manipulated, a new folder is created using the title method of "data-[manipulation technique]". The manipulated data is stored in this location for differentiation from its original form
	d. If downloaded data from an external or public source is being used, it is stored in a folder titled "data_dl". Include the data sourcenin the ReadMe file for reproducibility purposes

4. Metadata should be included and kept with all relevant data. Accompanied by a README that describes the data and metadata in an interpretible manner
	a. README should include links and/or DOI to relevant papers and preprints
	b. README should include contact information for authors and data creators, as necessay

5. Data is backed up in a *minimum* of two places (beyond personal computers and GitHub). This can be on an external hard drive, Rutgers Box, Amarel, or Annotate

6. In a scenario in which the data is too large to be stored on GitHub, it is deposited in the Pinsky lab Box account
	a. Additional back ups, such as through Amarel, Annotate, or an external hard drive are highly suggested

7. Data processing is accomplished through the use of computational scripts
	a. Helps to verify the reproducibility of computational biological methods
	b. 3rd-party data, not hosted by the Pinsky Lab, that is required to run scripts should be made accessible by providing links, descriptions for access/download, or otherwise add the data are required

8. Git repositories are published through [Zenodo](https://www.zenodo.org) accompanying the publication of a manuscript
	a. If the repo is included in a publication, please also archive it with a DOI on [Zenodo](https://www.zenodo.org) (see [here](https://github.com/pinskylab/pinskylab_methods/blob/master/cookbook.md#archiving-a-git-repo-with-zenodo-for-a-publication)).

9. Collaborative manuscripts are written in Google Drive

10. Presentations are typically made in Google Slides allowing lab members easy access to useful graphics

11. During matriculation ensure all projects, code, data, papers, etc. are uploaded in the Pinsky Lab organization on GitHub


##Data
------
Data used in support of a project must be:

1. Saved in an appropriate, non-proprietary format with accompanying metadata

2. In a public archive (e.g., the github repository or another public archive), or, if data is proprietary, a 'snapshot' version of the data used in the project must be saved in a private repository accessible to lab members

3. Linked and briefly described in the project README


##Code
------
Code used or developed in support of the project must be:

1. Well commented and complete

2. On Github, in the public project repository

3. Described in the README -> what does each file do, what language was used, what is the purpose of functions and parameters, etc.

4. Tested! Can at least one other person (more is better) complete your analysis on a different computer?
