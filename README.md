### Thermodynamic genome-scale metabolic modelling of metallodrug resistance in colorectal cancer

Mass spectrometry-based metabolomics approaches provide an immense opportunity to enhance our understanding of the mechanisms that underpin the cellular reprogramming of cancers. Accurate comparative metabolic profiling of heterogeneous conditions, however, is still a challenge. Measuring both internal and external metabolite concentrations we constrain four instances of a thermodynamic genome-scale metabolic model of the HCT116 colorectal carcinoma cell-line to compare the metabolic flux profiles of cells that are either sensitive or resistant to ruthenium- or platinum-based treatments. Normalizing according to growth rate and normalizing resistant cells according to their respective sensitive controls, we are able to compare the drug-specific metabolic responses of resistant cells. We find the normalization steps to be crucial in the interpretation of the metabolomics data and show that the metabolic reprogramming in resistant cells is limited to a select number of pathways.

This work is currently in submission. The Zenodo link for the work captured at the time of submission is: 
*insert DOI* 

The analysis can be re-constructed from the following Jupyter notebooks
- `growth_rate_analysis.ipynb`: Growth rates fitted to the experimentally determined cell counts 
- `metabolom_raw.ipynb`: Analysis of the metabolomics raw data 
- `exometabo_constrain.ipynb`: Using the measured exometabolite concentrations over time to fit exchange rates and to constrain the metabolic model 
- `metabolom_constrain.ipynb`: Used the pyTFA package and the experimentally determined metabolomics data to generate a thermodynamic model
- `flux_analysis.ipynb`: Analyses of the flux values calculated in the thermodynamic analysis 
- `seahorse_comp.ipynb`: Analyses of flux values calculated in the thermodynamic analysis with respect to energy metabolism 
- `hypoxia_simulate.ipynb`: For simulating hypoxic conditions using the previously generated model instances
- `FAlim_simulate.ipynb`: For simulating changes in fatty acid supply using the previously generated model instances 

#### Resources 

The `localpytfa` package was obtained from [Salvy et al. 2018](https://academic.oup.com/bioinformatics/article/35/1/167/5047753) (see [here](https://github.com/EPFL-LCSB/pytfa) for the code) and was adapted as described in the manuscript. 

The colorectal HCT116-specific genome-scale metabolic model was obtained from [Robinson et al. 2020](https://stke.sciencemag.org/content/13/624/eaaz1482) and compared to a combined model of the person-specific metabolic models produced by [Uhlen et al. 2017](https://science.sciencemag.org/content/357/6352/eaan2507). 

A link to the manuscript will be provided here upon publication. 
