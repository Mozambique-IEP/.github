# Mozambique IEP

This organization contains the code of the Open Source Spatial Electrification Tool (OnSSET) modified for the case of the Mozambique Integrated Energy Access Project, led by the Unidade de Planificação e Coordenação de Electrificação (UIPCE) in the Ministry of Mineral Resources and Energy of Mozambique (MIREME), supported by Sustainable Energy for All (SEforALL).



The organization contains the following repositories:



* **Clustering** - This repo is used to create the base layer population settlement clusters that are used for the geospatial electrification analysis
* **OnSSET\_GIS\_Extraction\_Notebook** - This repo contains the code required to extract data from the necessary GIS datasets to the population settlement clusters
* **onsset** - This repo contains two pieces of code: 1) Calibration is used to calibrate the demographic parameters and identify the settlements that are considered likely to be already electrified, 2) Scenarios is used to identify the least-cost technology (grid-connection, mini-grid or SHS) in each population settlement cluster to provide electricity access 



All three repositories are based on Python and Jupyter Notebook, and require the configuration of a Python environment. This is most easily achieved using Anaconda and the *moz\_onsset\_env.yml* file that is available in all three repositories. 

To install the environment using Anaconda, complete the following steps:

1. Clone or Download the repo to your computer
2. Open *Anaconda Prompt*
3. *Use cd* ... to move to the folder you have cloned or downloaded
4. Run the following command *conda env create --name moz\_onsset\_env --file moz\_onsset\_env.yml*
