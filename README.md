This repository contains the code used in my Summer Project for the MSc in Bioinformatics at the University Of Glasgow (2018-2019).
It was aimed at predicting structural fingerprints of Gene Clusters' products from genomic data.
All the code was written on Jupyter Notebook and, also, some data files are provided.
The "whole pipeline" notebook contains models already trained so the user can load a new Biosynthetic Gene Cluster (BGC) file from MIBiG (https://mibig.secondarymetabolites.org/#!/)
For this, the user needs to download both the GenBank file and the JSON file for a certain BGC (IMPORTANT THAT THE JSON FILE CONTAINS A SMILE STRING, NOT ALL OF THEM HAVE). The pipeline provides the user with the top 3 predictions from both  Machine Learning algorithms: Input Output Kernel Regression (IOKR) and Keras Neural Network.
Each folder has a README file which explain what each file is.
The rest of the machine learning scripts give as an output an "npy" file which contains a matrix that should be analysed with the script "analysingScores.ipynb" to know the percentage of times the expected output was set to be within each TOP.
