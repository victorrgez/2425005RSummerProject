This folder contains the main scripts of the project. These scripts were used for parsing the raw files that were eventually used as the input/output for the machine learning algorithms.
The "tryingKeras" notebook contains the instructions for running a Keras neural network with Pfam counts.
The "optimisedPaperFormula" notebook contains the instructions for running the IOKR algorithm with Pfam counts.
The "analysingScores" is used for analysing the score matrixes obtained with both machine learning algorithms. Takes a numpy matrix as an input and gives the user the percentage of times the expected output vector was set to be withing the Top 1, Top 3, Top 5, etc.
The input/output files can be found in the files folder.
In each script, the first line reads the purpose of each notebook.
