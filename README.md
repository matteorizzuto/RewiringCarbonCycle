# A theoretical framework for animal-driven carbon sequestration

This repository contains the code to replicate the numerical analyses of the model presented in Rizzuto et al. _Rewiring the carbon cycle: a theoretical framework for animal-driven ecosystem carbon sequestration_.

This repository contains the following items:

* in folder _Code_,
  - CarbonModelAnalysis.nb, this is the Wolfram Mathematica notebook we used to solve the model analytically, and to find the model's equilibria and expressions for the ecosystem processes of interest, which are used in the SupportingCode.Rmd R notebook in this folder. This file is also available in text format (.txt).

  - SupportingCode.Rmd, this is the R notebook where we numerically analyze our model, as described in the manuscript. It contains code to reproduce all figures in the manuscript. A compiled version of this file is provided as an HTML file.

  - Bibliography.bib, a bibtex file containing the references cited in the R markdown notebook.

* in folder _Data_,
  - pDATA1.csv, pDATA2.csv, cnDATA.csv, files containing data to run the model. The SupportingCode.Rmd file contains the code that was use to generate these .csv files.

* in folder _Results_,  
  - empty folder to collect results from running or knitting SupportingCode.Rmd; **note that this folder needs to be created before replicating the analyses, see below**

**Additional information on reproducing our analyses**

Information on the versions of R and of the packages used is provided in both versions of the SupportingCode file.

To reproduce our model analyses, please run all code chunks or knit the R notebook. Please note that the R notebook requires the following folder structure to work:

```bash
../
├── Code
├── Data
└── Results
```

Any change to the structure of the folder needs to be reflected in the relative paths used throughout the R notebook. A simple search for “../“ should suffice to find all instances in which relative paths are used and to update them as needed.

The code presented in CarbonModelAnalysis.nb can be used in Wolfram Mathematica to find the model’s equilibria. An alternative .txt version of this notebook can be perused, if Wolfram Mathematica is not available.
