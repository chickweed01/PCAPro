<img src="/images/pcapro-app-icon.png" align="left" />

# PCAPro

Principal component analysis (PCA) is a data analysis step step in the process of creating a machine learning model. Often times the analyst is presented with a dataset having many features. Instead of attempting to fit the entire set of features into an ML model the analyst has the option of first identifying which features account for the most variance in the data. This gives the analyst the opportunity to reduce the number of features in the ML training dataset while preserving as much of the information in the data as possible.

PCA Pro performs an eigenvector transformation of a ML dataset. It first standardizes the dataset so that the data values in each column have a mean of zero and a standard deviation of one. Next, a NxN correlation matrix is constructed from the standardized dataset where N is the number of features in the dataset. Eigen decomposition is then performed on the covariance matrix to calculate the eigenvalues and eigenvectors.

Typically, the analyst would then sort the components in descending order of their eigenvalues and produce a scree plot showing the accumulated percentage of variance accounted for by each component. These are now referred to as the principal components. The analyst then decides to keep the first M components where M <= N. A transformation matrix is constructed whose columns are the M eigenvectors.

See the <a href="/about.md">About</a> page for further info and the <a href="/PCAProHelp.pdf">Help</a> doc for "how-to" instructions.
