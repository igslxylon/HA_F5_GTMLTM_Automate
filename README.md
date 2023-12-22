![image](https://github.com/igslxylon/HA_F5_GTMLTM_Automate/assets/68359513/5599b176-6dbc-4838-b8e7-d4486b6efb44)# Project HA_LTMGTMAutomate
## Overview
The program is to transform GTM Excel `ltm-gtm-template.xlsx` to several ansible variables yml file.
## Install
1. Clone the project .zip file and extract to a folder, `{project_home}`
2. Install the python module
```
pip install pandas
pip install pyyaml
pip install PyGithub
pip install ruamel.yaml
```
3. Execute Script
```
cd {project_home}
python ./GTMTaskAutomate.py
```
## Folder Structure
```
.
├── config                      # Config Folder
    ├── GTMConfig.py            # File, Config Variables stored for Input, Output and Github parameters
    ├── logging.conf            # File, Logging Conf File
    ├── Service_DC_Mapping.csv  # File, CSV storing the Serivce, Server Info and Data Center Mapping
    └── ...
├── output                      # Destination Folder for output ansible variables yml files
    └── <tsr_no>                # Folders, naming with <tsr_no>, e.g. 
├── service                     # Service Folder for Service module storing ansible variable pattern
├── template                    # Template Folder for YML Template of Ansible Variable
├── util                        # Tools and utilities
├── ltm-gtm-template.xlsx       # File, The Excel File provided by User
└── README.md
```

