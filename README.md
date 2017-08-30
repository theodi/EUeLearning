# EUeLearning

This repository contains the live deployed source code for the 13 eLearning modules hosted on the European Data Portal.

https://www.europeandataportal.eu/elearning/en/#/id/co-01

These modules are built using the Adapt eLearning framework version 1 (now deprecated).

There are two ways to edit these modules:

1) By directly editing the version hosted here - Recommended to update those modules on the European Data Portal. 

2) By setting up your own Adapt eLearning environment and using the course source files to build a new course - Recommended if you want to significantly re-use the content to build a new course. 

Each method is outlined briefly below.

## Method 1 - Direct editing

To directly edit the modules to make changes without requiring a copy of the full adapt framework follow the steps below.

1) Fork a copy of this GitHub repository. 

2) Edit the source files in the course/{lang} folder, where the language is either en or fr. 

Guides on the structure and contents of each file can be found on the [Adapt Wiki](https://github.com/adaptlearning/adapt_framework/wiki/Creating-your-first-course). Note that you will not require to rebuild the course using the `grunt` tools when directly editing. 

Editing in this way is limited to the content. The look and feel and source code for the tool are not as straight forward to edit due to the fact that these files are compiled in order to save space. This means that the EU tracking code remains and statistics will be reported to the EU analytics engines.

## Method 2 - Setting up your own Adapt eLearning environment

IMPORTANT: At the time these modules were created the latest version of the Adapt eLearning environment was version 1. In order to reuse the modules most effectively it is recommended you use Adapt version 2 (as outlined here) and follow the migration guide.




The master repository with the source code is located at https://github.com/theodi/ODI-eLearning

Please file any issues there rather than here. 

Thanks!
