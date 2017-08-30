# EUeLearning

This repository contains the live deployed source code for the 16 eLearning modules hosted on the European Data Portal.

https://www.europeandataportal.eu/elearning/en/#/id/co-01

These modules are built using the Adapt eLearning framework version 1 (now deprecated).

This guide covers:
1. How to deploy these modules as SCORM objects
2. How to direcly edit these modules
3. How to set up your own development environment using these modules. 

## 1. How to deploy these modules as SCORM objects

The SCORM objects can be downloaded from each individual module at https://www.europeandataportal.eu/elearning/en/#/id/co-01. 

The SCORM object downloads are available from the Open Data section of the Menu.

*Note 1*: The SCORM objects are direct builds of the EU version and contain the theme and all customisations (including analytics and tracking)

*Note 2*: The SCORM objects are avaialble under an Open Licence however this licence *DOES NOT* cover third party rights including shutterstock images and company logos. Re-users should establish their own rights to use such contents prior to direct re-use. 

## 2. How to directly edit these modules (Recommended to update those modules on the European Data Portal)

To directly edit the modules to make changes without requiring a copy of the full adapt framework follow the steps below.

1. Fork a copy of this GitHub repository. 

2. Edit the source files in the /{lang}/moduleX/course/{lang} folder, where the language is either en or fr and the X in module X in the module number.

Guides on the structure and contents of each file can be found on the [Adapt Wiki](https://github.com/adaptlearning/adapt_framework/wiki/Creating-your-first-course). Note that you will not require to rebuild the course using the `grunt` tools when directly editing. 

*Note 1*: Editing in this way is limited to the content. The look and feel and source code for the tool are not as straight forward to edit due to the fact that these files are compiled in order to save space. This means that the EU tracking code remains and statistics will be reported to the EU analytics engines.

*Note 2*: The course objects (in /course/{lang} are avaialble under an Open Licence however this licence *DOES NOT* cover third party rights including shutterstock images and company logos. Re-users should establish their own rights to use such contents prior to direct re-use. 

## 3. How to set up your own development environment using these modules.

IMPORTANT: At the time these modules were created the latest version of the Adapt eLearning environment was version 1. In order to reuse the modules most effectively it is recommended you use Adapt version 2 (as outlined here) and follow the [migration guide](https://github.com/adaptlearning/adapt_framework/wiki/Converting-a-Course-from-Version-1-to-Version-2).

1) Set up your own Adapt 2 environment following this [guide](https://github.com/adaptlearning/adapt_framework/wiki/Setting-up-your-development-environment).

2) Create your first course as per the guide.

3) Overwrite the files in the course directory with those from the /{lang}/moduleX/course/{lang} directory of your selected module. Note that all modules have been set up as separated courses for easy of editing in this way. To set up a single Adapt 2 course all of the source course/{lang} files will need to be merged into a single directory (not recommended). Note that you will have to follow the migration guide to make the courses work properly in Adapt 2 using the [migration guide](https://github.com/adaptlearning/adapt_framework/wiki/Converting-a-Course-from-Version-1-to-Version-2). 

4) [Optional] The european data portal theme is available [here](https://github.com/theodi/adapt-theme-eu/blob/master/README.md). This can be used as a custom theme by downloading it into the adapt_framework\src\theme\ directory. More information on themes and using themes can be found on the [Adapt Wiki](https://github.com/adaptlearning/adapt_authoring/wiki/Modifying-the-Vanilla-Theme).  

*Note 1*: The course objects (in /course/{lang} are avaialble under an Open Licence however this licence *DOES NOT* cover third party rights including shutterstock images and company logos. Re-users should establish their own rights to use such contents prior to direct re-use. 

*Note 2*: The original master repository with the source code (including Adapt 1 framework) is located at https://github.com/theodi/ODI-eLearning. However, we would not recommend using this! As Adapt 1 has now been retired there is very little support (other than bug fix) for developing using this old version of the framework.

Thanks!
