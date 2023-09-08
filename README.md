# InVesalius fMRI Support Documentation

In this section we provide support for fMRI volumes. From BIDS format fMRI datasets we extract information from the BOLD timecourses and overlay such information:

- Functional Slice
- General Parcellations (e.g Yeo7, Yeo17)
- Functional Connectivity (allowing seed based correlations)
- Functional Gradients

Such volumes can be loaded in the Invesalius UI and overlayed onto T1 volumes to provide further insights during neuronavigation.

### Descriptions
- main.py: main script to run the processing
- load_resources.py: functionals used to download volumes necessary for processing
- tool_processing.py: class used for processing the downloaded volumes and generate UI compatible volumes
- resources: location of the generated volumes
- tutorial: example of usage
- tutorial-fmri_processing.ipynb: example of usage through notebook
  


### Instructions
General library requirements are that of Invesalius.
In addition we require the installation of AntsToolBox and fmriprep (only used in the tutorial)

Installation resources:
- AntsToolBox: https://github.com/ANTsX/ANTs/wiki/Compiling-ANTs-on-Linux-and-Mac-OS
- fmriprep: https://fmriprep.org/en/20.2.0/installation.html

```console
conda activate invesalius
python3 main.py
```

To have a more intuitive understanding of the pipeline do recommend checking out

```console
conda activate invesalius
python3 -m jupyter notebook
```

### CITATION
The tutorial dataset employed can be found on on openneuro (https://openneuro.org/datasets/ds000102/versions/58016286cce88d0009a335df)

Kelly AMC and Uddin LQ and Biswal BB and Castellanos FX and Milham MP (2018). ds000102. OpenNeuro. [Dataset] doi: null