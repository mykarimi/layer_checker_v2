# Layer Checker version 2.0
A script that checks if all the possible layers with nlp information are present in the NAF-output file generated by the nlp-pipeline. 

- Author: M. Yassine Karimi
- Date: October the 2nd, 2015
- Vrije Universiteit Amsterdam

##Requirements
- OS X or Linux OS (UbuntuGNOME v14.02 for example) installed
- Installed version of Python 2.7 or higher (script was built on v2.7)
- KafNafParser for Python (https://github.com/cltl/KafNafParserPy)
- Terminal (comes with Linux OS)
- XML v1.0 or higher
- Text editor (Sublime Text 2, gedit)


##Setup
Download the complete github repository with the follwing command:

            - git clone https://github.com/mykarimi/layer_checker_v4

In order to be able to use layer_checker_v2, the KafNafParser - which is required for this script to work - must be set to the right path;
- Open the script with a texteditor (sublime text 3, gedit, or any other)
- Go to line 22 and find

            22 sys.path.append('/locaton/of/my/KafNafParser')
            23 from KafNafParserMod import *

- Change the location in sys.path.append() to the location of your KafNafParser

##Usage

- open the terminal

- In order to run layer_checker_v2.py, you must go to the folder (downloaded repository) of the the             layer_checker_v2 Place the file(s) that you want to proces with the script in the input folder:
            
            cp /original_folder/sample_naf_file.naf /folder_where_the_repository_is/layer_checker_v2/input/
            mv /original_folder/sample_naf_file.naf /folder_where_the_repository_is/layer_checker_v2/input/

- Then go to the main folder of the repository 

            cd /folder_where_the_repository_is/layer_checker_v2/
            
- ...and run the script with the following command.

            python layer_checker_v2.py
