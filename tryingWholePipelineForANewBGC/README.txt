	The "wholePipeLineForANewFileWithModelsTrained" notebook has a pipeline which currently reads
both the GenBank and JSON files of the cluster 1720 and creates the Pfam counts vector
and the fingerprint one and uses both the IOKR algorithm and Neural network with models
already trained. However, the keras model file "neuralnetworkmodel.h5" cannot be uploaded
to GitHub since it is more than 500mb. This part of the script can be commented out
for this reason. The file "testSetIndexes" has the order of the fingerprints that were
included in the test set when training the model. This is important if we want to try
the pipeline with a new BGC, so we make sure we use one of these which were not included
in the training set. Also, the set of possible output vectors for the ranking of the fingerprints
is taken from these files. "List of Domains" is the list of 6159 pfam domains included in the
pfam count vectors in alphabetic order (same order that was used for the input files with 0s and 1s.
The "hmmeroutput" file for BGC 1720 has been provided in case the user does not have hmmer installed
in their computer. This way, BGC 1720 will still report results. The hmmer line is currently
commented out therefore in the jupyter notebook script. Smart molecules has the substructures from CDK
except for the substructure 298 which always gave an error with RDKit.
