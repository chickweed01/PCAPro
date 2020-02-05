<img src="/images/pcapro-app-icon.png" align="left" />

# PCAPro

Principal component analysis (PCA) is a data analysis step in the process of creating a machine learning model. Often times the analyst is presented with a dataset having many features. Instead of attempting to fit the entire set of features into an ML model the analyst has the option of first identifying which features account for the most variance in the data. This gives the analyst the opportunity to reduce the number of features in the ML training dataset while preserving as much of the information in the data as possible.

PCA Pro performs an eigenvector transformation of a ML dataset. It first standardizes the dataset so that the data values in each column have a mean of zero and a standard deviation of one. Next, a NxN correlation matrix is constructed from the standardized dataset where N is the number of features in the dataset. Eigen decomposition is then performed on the covariance matrix to calculate the eigenvalues and eigenvectors for each component.

Next, PCA Pro sorts the components in descending order of their eigenvalues and produces a scree plot showing the accumulated percentage of variance accounted for by each component. These are now referred to as the principal components. The analyst then decides to keep the first M components where M <= N. PCA Pro constructs a transformation matrix whose columns are the M eigenvectors. The origional dataset matrix is then multiplied by the transformation matrix. If the origional dataset is P rows by N columns and the transformation matrix is N rows by M columns, the resulting transformed dataset will be PxM where M <= N.

See the <a href="/PCAProHelp.pdf">Help</a> doc for "how-to" instructions.
