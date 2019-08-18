	This folder contains the most important results of the project.
	K-mers and Pfam counts files were tried as inputs for both neural network and IOKR.
	Pfam counts with IOKR obtained the best scores with a top 1 better than 35% (keepingTrackOfResultsForIOKRPfam).
	Other results are shown in the other files.
	Additionally, the callback graphs is a record of the loss function
and binary accuracy of different optimisers using the callback CSVLogger from the keras neural network
	KeepingTrackOfCategory results are the scores obtained for different categories of gene cluster products,
according to the category shown in the json files from MIBiG. Saccharides are predicted with higher accuracy.