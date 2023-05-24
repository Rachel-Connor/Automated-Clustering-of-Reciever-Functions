# Automated-Clustering-of-Reciever-Functions
This repository follows the development of my Final Masters Project. The project aims to build an automated clustering algorithm that clusters pre-processed seismic receiver functions in Iceland based off of BAZ and epicentral distance. 

The data for this project is provided by an Earth Science Professor at Durham University who specialises in sesimic activity. The raw data (in the form of sesimograms) was collected by 160 seismic stations distributed throughout Iceland. These seimograms were then preocessed by the aforementioned expert who then enlisted technical help to automate the clustering process using cleaned Reciever funcitons. The Reciver Functions themselves are stored individually before the iterative deconvolution process as PICKLE files. They can be accessed using obspy and presented by use of a personalised function. 

The aim is to cluster the receiver functions according to BAZ and epicentral distance by station. Therefore, though the dataset is large, the input for each cluster is small - averaging 17 functions per station, with 2 relevant features. As this dataset is not an ideal candidate for feature-reduction, the pre-processing task is small though the relevant features need to be extracted for each receiver function using the obspy stats command.

The clustering algorithms used in this project will be K-Means, Hierarchical and GMM. There is also a possability for an extension that would make use of an autoencoder to cluster the entire dataset as a whole wihtout station restrictions. 
