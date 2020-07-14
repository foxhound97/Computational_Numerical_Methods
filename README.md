# Computational_Numerical_Methods
Authentication based on a person’s face is one of the most stringent measures to secure a place or system. In this report such a method has been proposed that successfully identifies a person. The proposed algorithm also identifies a person with different emotions/varied face expressions. The algorithm first converts the RGB image into grayscale and then reshapes it into a 100 x 100 matrix by interpolation.  We flatten those matrices into vectors and stack them into a matrix called Data Matrix and compute its SVD to extract the Eigen-Vector matrix. 
We apply the Hadamard Product based transform on both Data Matrix and the Query Vector (Query image is flattened to vector with the same process mentioned above) with the Eigen-Vector Matrix. Computation of the difference between transformed Query Vector with each column of Transformed Data Matrix is performed followed by  norm. The Lowest Value is retrieved.
Due to the Preservation of Eigen-Vector matrix, the features of each image are highlighted, and hence, they give accurate results while comparing.

Result & Analysis:

1.By using the Eigen-Vector matrix U, obtained from the SVD of Training Matrix, to perform a Hadamard Product Based transform to detect the image(s) similar to that of the Testing Image within the Training Data Set, this approach yields efficient and enhanced results as compared to other face recognition algorithms.

2.Our algorithm can match similar faces even if the person in the image has different expressions in the dataset.

3.Also, it will yield accurate results even if the person is wearing glasses or any other face obstacle objects.

4.Even if the images of the same person are taken during different lighting conditions, the person is being recognized correctly.

5.These are few of the advantages that make this SVD based approach robust.
