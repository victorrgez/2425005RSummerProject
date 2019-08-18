	This folder contains different types of fingerprints used in the final phases of the project.
	Also, "pfamDomains0and1ForAllClusters" and "fingerPrintsForIndividualClustersNOT478"
are the most important files for the machine learning algorithms (input and output that got the best scores, especially with IOKR)
	These files do not contain the BGC 478 because no pfam domains were detected on it.
	The fingerprints for individual clusters correspond to the CDK ones whose substructures' smart strings
were obtained from "http://cdk.github.io/cdk/1.4/docs/api/org/openscience/cdk/fingerprint/SubstructureFingerprinter.html"
	All duplicated clusters were removed:
		-1031 clusters were included
		-CDK fingerprints are 306 bits long
		-Pfam counts are 6159 bits long
	The simplified fingerprint only contains the position 13 of the fingerprints as it is around 50% of the times a 1 and 50% of the times a 0. It was used for debugging the neural network, comparing its performance with other algorithms from Scikit-learn.
	"AllFingerprintsCombined" was a trial in which all fingerprints were combined into the same file to see if the scores were increased but it was not successful as the predictions were worse.
	The other types of fingerprints were obtained either from RDKit or with this script: https://github.com/hcji/PyFingerprint
	"FingerprintsWithoutOnly1or0positions" was a trial in which all those columns which were more than 99% 1s or 0s were deleted in order to remove noise, however the results were slightly worse than with the original fingerprints.
	The file "everycds.fasta" can be downloaded from "https://dl.secondarymetabolites.org/mibig/mibig_prot_seqs_1.4.tar.gz" and be renamed to everycds.fasta so it can be used for creating pfam counts and amino acid k-mers. It cannot be stored on github as it is big.
	All the fingerprints were obtained with the individual scripts included in "other scripts" folder and then the script "removingDuplicatedClustersForAllTypesOfFingerprints" found in "mainScripts" was used to remove duplicated clusters.
