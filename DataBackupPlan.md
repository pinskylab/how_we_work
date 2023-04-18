Data Backup Plan
================
### v1.0.0

### GitHub, Box, and the RAID
One of the fundamental reasons to have a backup and/or backup plan is to restore lost data in the
event of an emergency, a mistake, or an accident. In the Global Change lab group we follow the
3-location backup system by storing our files on GitHub/Google Drive, Box, and using our 16TB
(Cine)RAID storage tower as a physical backup. As well, to keep our data easy to navigate and
access we utilize a unified naming convention across all platforms with the intent of each
location being a near-identical copy to the others.

The lab group Google Drive and website are backed up to Box on a monthly basis, along with
any changes made to GitHub over the past month. These backups are then also stored in the
RAID. It is personal responsibility to backup your files to a project GitHub repo and any large
files to Box. All locations should also include a README describing the available files.

### Using a personal GitHub
To promote open-access to science, data traceability, and ensuring that all data is backed up in a
secure location, we ask that you maintain a GitHub repository on the Pinsky Lab group
organization. This should be done on a project-by-project basis. There are no issues with forking
the repo to your personal GitHub account or maintaining a secondary copy of the repo on a
personal account. However it is imperative that the primary repo be stored on the Pinsky Lab
GitHub.

### Shared naming on GitHub and Box
To promote a unified storage plan, GitHub repos are named based on the associated/planned
project. The repo name is then used as the name for the parent directory of the data backup on
Box and the RAID.

### Important files to backup
Please review the Pinsky Lab Data Management Plan for more information.
* Raw data
* Scripts
* Metadata

### What is Metadata?
Metadata has been described as “the data about data”. It contains relevant information
and description to the (raw) data. In many circumstances it can be utilized as a resource to help
with explaining and understanding analyses. Regardless of metadata’s importance, it may be the
most commonly overlooked source of information when discussing backups. It is essential to
back up any and all metadata for projects.

## Projected Backup Schedule

### Daily
* Personal upload of current scripts to GitHub
* Personal upload of working files to GitHub and/or Box
  * Less than 25MB to GitHub
  * Greater than or equal to 25MB to Box in reponame/data_largefiles
* Personal update the README files

### Monthly
* In the “Backups” dir on Box, create a new dir with the date of the scheduled backup
* Download and upload to aforementioned dir
  * Lab Google Drive
  * Lab Website
  * Lab GitHub repos with new commits within the past month
* Download the dir to the RAID

### Biannually
* Download all repos from the lab group GitHub
  * Store in Backups/GitHub dir on Box
* Talk with lab members about temporary files or intermediate files on cluster
* Do any files on the cluster need to be backed up?
* Can any files be deleted to ensure there is sufficient storage space?

### Yearly
* Clean up backups
* Remove unwanted backups over a year old
