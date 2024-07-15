# GCRG Lab Data Management Plan

The Global Change Research Group strives for an open science policy that makes our science accessible and reproducible and that allows us to collaborate with our future selves and with our colleagues. To assist in achieving that aim, we use the following practices.


## General project organization

1. Lab notebooks are maintained each day; tracking progress, daily learnings, what was accomplished, and/or what goal was worked towards. These can be physical notebooks, text files, Evernote, Jupyter notebooks, etc.
   1. Lab notebooks are digitally backed up, regardless of initial format

1. Each new project gets a GitHub repository in the [pinskylab organization](https://github.com/pinskylab)
   1. This practice facilitates collaboration, sharing, and maintenance of institutional knowledge
   1. Repos can be public or private
   2. A [CITATION.cff](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files) clarifies how to cite the repo. We apply authorship criteria similarly as for papers (e.g., first author is the lead).
1. Data processing is accomplished through the use of scripts, not manual manipulation
   1. This helps to verify the reproducibility of our methods
1. A README.md in each directory (including the top directory) 
   1. explains the purpose of each file and sub-directory
   1. includes links to relevant papers and preprints
   1. has contact information for authors and data creators, as necessary
   1. defines data columns, including units, of any data files and basic methods used for data collection
   1. has version numbers of any software or packages needed for running codes or scripts
1. If the repo is included in a publication, we also archive it with a DOI on, for example, [Zenodo](https://www.zenodo.org) (see [here](https://github.com/pinskylab/pinskylab_methods/blob/master/cookbook.md#archiving-a-git-repo-with-zenodo-for-a-publication) for instructions).
2. We add a license to each git repo, e.g., MIT or CC BY-NC 4.0, to clarify how the material can be reused. See guidance from [Creative Commons](https://creativecommons.org/share-your-work/cclicenses/), [Github](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository), and [R Packages book](https://r-pkgs.org/license.html#code-you-write).
3. We write collaborative manuscripts in the GCRG Shared Google Drive
4. Presentations are typically made in Google Slides in the GCRG Google Drive (Presentations/) allowing lab members easy access to useful graphics
   1. Name the file in the format YYYY-MM-DD_presentername_occasion, eg, 2023-01-07_Pinsky_AmNat
5. Before matriculation, we ensure all projects, code, data, papers, etc. are uploaded and fully documented

## Data
Data used in support of a project is:

1. Saved in an appropriate, non-proprietary format with accompanying metadata (e.g., csv rather than Excel)
1. Raw data is stored in or linked from the GitHub repository associated with the project
   1. Raw data files under the Github file size limit (<100MB) are stored in a data/ directory
   1. Larger files are stored in a data_largefiles/ directory (not tracked by Git by using the .gitignore file) in at least two places 
         - where the analysis is occurring (e.g., scientific workstation), and
         - on the UCSC PbSci Bishop data server in GCRG directory, in the data_largefiles/ directory, in a subdirectory whose name matches the Git repo name. When we do this, we document this arrangement clearly in the relevant data_largefiles/README.md file of the git repo.
   1. If data from an external or public source is being used, it is stored in a data_dl/ directory (not tracked by Git). We clearly and unambiguously describe the data source in the data_dl/README.md file by providing links, version numbers, descriptions for access/download, or other details to ensure reproducibility. If you're worried the data won't be available in the future, follow one of the two previous bullet point approaches.
   2. Sequencing data is something of a special case. We upload our raw reads to NCBI soon after receiving them, possibly with an embargo, with the accession numbers documented in the relevant README.md. If this is not possible, we keep a copy of the reads on Box in data_largefiles/ in addition to the copy on the scientific workstation where the files are being processed. 
   3. Metadata is stored in the same directory as the raw data, typically in a README.md file that describes the data in each column, units, coordinate reference system (CRS, for GIS data), and other details needed to understand the file
   4. Processed or cleaned data is stored in a separate directory, e.g., output/ or similar, to differentiate from raw data


## Code
All code used or developed in support of the project is:

1. Well commented and complete
1. Versioned in the project's git repository
1. Described in the README.md file to explain what each script does, what language was used, what software and package versions were used, etc.
1. Tested! Can at least one other person (more is better) complete your analysis on a different computer?

## Backups
We store our raw data and scripts in at least two locations.

1. Most of our work is on Github or Google Drive. Both are backed up monthly to Box and to an external harddrive by a designated lab member.
1. Raw data files too large for Github and Drive are stored on the scientific workstation on which they are being manipulated or posted on Figshare, then manually copied to Box by the researcher (use a directory with the same name as the parent Git repo and subdirectory named data_largefiles/). They are backed up from Box monthly to an external harddrive by a designated lab member.
