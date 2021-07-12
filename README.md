# Principal-Component-Analysis
Part 1 : Standardization of Data

The purpose to standardise the data is to prevent some features from having a dominant effect on the resultant vectors. To have standardized data for different features, data normalization is applied to the data. The new data will be the result from old data minus the mean of that feature and divide with its standard deviation. After this normalization, all the data will be transformed in the same scale.


Part 2 : Compute Covariance Matrix

The purpose of this is to express the correlation between the different variables in the data set. It is essential to identify heavily dependent variables because they contain biased and redundant information which reduces the overall performance of the model. Mathematically, a covariance matrix is a p × p matrix, where p represents the dimensions of the data set. Each entry in the matrix represents the covariance of the corresponding variables. 


Part 3 : Compute Eigenvalue and Eigenvector

An eigenvector is a nonzero vector that changes at most by a scalar factor when that linear transformation is applied to it. The corresponding eigenvalue is the factor by which the eigenvector is scaled. 


Part 4 : Sort the Eigenvalue and Eigenvector

The purpose of this is to ensure that the eigenvectors are sorted in descending order to their eigenvalue. Hence, we can get the eigenvector that preserves the highest amount of information.


Part 5 : Transform to Original Matrix

Pick k eigenvalues equal to 1 and form a matrix of eigenvectors which we have got from the output of the svd method. Transform the original data by compute the projection of data using only top K which is 1 eigenvector like example U[:, K] where U is eigenvectors and multiply with the original matrix.
