# Mozambique IEP

This organization contains the code of the Open Source Spatial Electrification Tool (OnSSET) modified for the case of the Mozambique Integrated Energy Access Project, led by the Unidade de Planificação e Coordenação de Electrificação (UIPCE) in the Ministry of Mineral Resources and Energy of Mozambique (MIREME), supported by Sustainable Energy for All (SEforALL).



The organization contains the following repositories:



- **"Clustering"** - This repo is used to create the base layer population settlement clusters that are used for the geospatial electrification analysis. The rationale behind the selected code is described in this [pptx (Coming Soon)](https://example.com)
- **"OnSSET\_GIS\_Extraction\_Notebook"** - This repo contains the code required to extract data from all the necessary GIS datasets to the generated population clusters (settlements) from the previous code. The code works with sample data at the moment. Running the code at national level require data that cannot be stored on GitHub due to size, but they are available upon request to the UIPCE team. **Note!** The data will become available via the Mozambique IEP Spatial Data Infrastructure (SDI), which is currently under development.
- **"onsset"** - This repo contains two pieces of code:
  * 1) **"Calibration"**, which is used to calibrate the input GIS demographic parameters to the official country statistics, covering population counts, urbanization status and electrification status.
  * 2) **"Scenarios"**, which is used to run least-cost electrification scenarios. This model yields the least-cost technology (grid-connection, mini-grid, or SHS) for each settlement, given specific inputs/targets, as well as the capacity and investment needed to achive deployment of these technologies in the specified timeframe.


All three repositories are based on Python and Jupyter Notebook, and require the configuration of a Python environment. This is most easily achieved using Anaconda and the *moz\_onsset\_env.yml* file that is available in all three repositories. 

To install the environment using Anaconda, complete the following steps:

1. Clone or Download the repo to your computer
2. Open *Anaconda Prompt*
3. *Use cd* ... to move to the folder you have cloned or downloaded
4. Run the following command *conda env create --name moz\_onsset\_env --file moz\_onsset\_env.yml*
