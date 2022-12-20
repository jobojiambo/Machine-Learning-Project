# Machine-Learning-Project
A K-Means Clustering Algorithm.
Project Report:

Project Purpose:
For decades, the Banking sector has perpetually been faced with the challenge of counterfeit banknotes. In this project, I used machine learning to model a simple algorithm that can automate the process of detecting counterfeits from the real banknotes. 

	Dataset Description
Sourced from OpenML with Wavelet Transform used to extract special features from real and counterfeit banknote images, the data is contained in a csv file with 1372 rows 2 columns V1 and V2. Where:
V1 represents the Variances of the Wavelet Transform images, and
V2 represents the Skewness of the Wavelet Transform images.
(Note that n = 1372)

	Analysis Method Description
In this project, I used K_means clustering as the machine learning algorithm to analyse the Banknote data. I  repeated the clstering process by first creating 5 clusters, then 4 clusters and finaly settling on 2 clusters (to represent genuine or fake banknotes). Furthermore, I had to normalize my dataset for better and more visually desirable results.

Summary of Results (Findings):
Using the Numpy Python library, I was able to deduce the following from the dataset: 
For V1 (Variances): 
The mean is 0.43, the standard deviation is 2.84, and the range of the data is between -7.042 (min) and 6.825 (max).
For V2 (Skewness):
The mean is 1.92, the standard deviation is 5.87, and the range of the data is between -13.773 (min) and 12.952 (max).
After the data was normed I was able to obtain the following scatter plots:


Before runing K-Means algorithm:

 

After Running K-means Algorithm using code:
km_Res = KMeans(n_clusters = 2).fit(Range_V1)
print([km_Res, Range_V1])
 
To ensure stability of the results, I ran K-means 10 times.
Recommendations
Despite getting exemplary results from the K-means Machine Learning model, it is my opinion that the results could be improved. To provide room for improvement it is my recommendation that the number of samples be increased (especially the number of counterfeits) so as to furnish the algorithms with as much data as possible to chew and spit out the most desirable results.

























