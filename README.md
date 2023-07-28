# The Diffusion MRI lexicon (DiffusionLex)  

## Overview 

The ISMRM Open Science Initiative for Perfusion Imaging (OSIPI) has developed a lexicon for contrast-agent perfusion MRI (CAPLEX). This lexicon was first developed using googledocs, but has now been migrated to a webpage hosted by github pages. The aim of the lexicon is to define standard terminology for quantities, models and processes used in perfusion MRI to reduce reporting variability. Through this effort, a general framework has been developed for lexiconography applied to MRI data. This repo hosts an extension of the OSIPI CAPLEX to diffusion MRI.  

## Repository contents
The repo is in development but currently contains:

1. the "editable" markdown (.md) files that define the diffusion lexicon content (e.g. the webpage content in the **/docs** directory).
2. the "non-editable" backend for the DiffusionLex webpage generated when .md files on main are deployed (found on the **gh-pages** branch)

## Contributing to the lexicon
The lexicon is designed to the extensible and we actively engage researchers in diffusion MRI field to engage with its usage and development. If you would like to add or edit content (new entries etc.) of the lexicon, please either:
1. contact Ben Dickie (ben.dickie@manchester.ac.uk) with your proposed changes. 
2. or create a development branch of main and edit the .md files directly. Once done, submit a pull request (do not merge with main!), which will then be reviewed by the core development team. 
3. or fork the repo, make the changes you want to make, then push back to the parent repo. This is recommended if you make regular changes. 

## Suggesting edits or additions to lexicon entries

Edits or altogether new entries can be suggested by editing the .md files found within the **/docs** directory. To do this, make a new *development* branch of main and edit the .md files as necessary. Some basic instructions on how to edit markdown files are given here: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

Once done, commit the changes and submit a pull request. Make sure to add a description of the changes when making the pull request. 

## Deploying changes
After careful review, proposed changes to markdown files made on a development branch will be merged into the *main* branch. After the merge is approved, this will trigger a CI workflow to automatically generate the new docs and publish to the *gh-pages* branch, **which should not be edited manually**.

