# Layer Checker version 2.0
A script that checks if all the possible layers with nlp information are present in the NAF-output file generated by the nlp-pipeline. 

- Author: M. Yassine Karimi
- Date: October the 2nd, 2015
- Vrije Universiteit Amsterdam

Steps:

In order to be able to use the layer, the KafNafParser must be set to the rigcht path;
- Open the script with a texteditor (sublime text 3, gedit, or any other)
- Go to line 22 and find

      sys.path.append('/locaton/of/my/KafNafParser')
      from KafNafParserMod import *
