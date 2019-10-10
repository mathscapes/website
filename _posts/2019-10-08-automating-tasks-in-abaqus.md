---
layout      : post
title       : Automating tasks in ABAQUS
author      : "Rahul Singh"
tags        : ["ABAQUS", "Python", "Scripting"]
cite        : true
---

Python scripting allows ABAQUS[^1] users to efficiently execute and automate specific tasks, which researchers sometimes classify as manual labor. Users can code specific tasks using Python scripts and can be run from File → Run Script. 

The information regarding the objects and methods used can be found in the ABAQUS Documentation. ABAQUS Documentation contains scripting examples for basic scripting. The example scripts linked in this article explores the visualization and data extraction from ODBs and a few utility scripts to enhance productivity. 

## Copying parts
This small piece of utility script can be used to copy parts attributes like mesh, section assignments, orientation, etc.

One can make a part and use this script to create multiple copies. If you modify a part, you can rerun the script to maintain uniformity, and the same will be updated in the Assembly. 

## Data extraction and visualization

This script can be used to extract field and/or history output data from ABAQUS ODBs. If you have a set of jobs, you can create a List (here LamN), which can be called in using for loop to open, extract and close the ODBs one by one.

This script also allows you to maintain a consistent naming scheme for job lists e.g., JB-CP1v250. JB is a tag, CP1 being the model code and 250 could denote a specific loading condition. 

Nested could be used to execute if you have more than one set of models and loading conditions, creating combinations.

The script is written for a particular case i.e., impact loading of plates. Major parameters like Residual velocity, Time is taken to reduce the energy of projectile to 0, Displacement of Projectile/indentor, etc. can be extracted from the ODB. The extracted data is written in a separate CSV file for post-processing. 

Example scripts can be found [here](https://github.com/mathscapes/mpart).

## References
[^1]: Abaqus FEA (formerly ABAQUS) is a software suite for finite element analysis and computer-aided engineering.