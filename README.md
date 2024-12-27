# PA-Project  
To implement a parallel version of the KNN algorithm, we leveraged parallel processing techniques to speed up the computation. One of the most straightforward ways to parallelize the KNN algorithm is to parallelize the distance calculation and the nearest neighbor search. We can used Python's multiprocessing library "joblib" to achieve this.   
Here, I'll use joblib to parallelize the distance calculation and nearest neighbor search. This will allow us to distribute the workload across multiple CPU cores, making the computation faster.


**Parallelization with joblib:**   
We use joblib.Parallel to parallelize the prediction for each test point. The delayed function is used to create a parallel job for each test point.


**Distance Calculation and Nearest Neighbor Search:**   
The distance calculation and nearest neighbor search are performed for each test point in parallel.

**Benchmarking:**   
The code measures the time taken for the parallel KNN prediction and compares it with the non-parallel version.

**The code files:**   
The repo contains two jupyter files, one for the non-parallel approach and one for the non-parallel approach.

**Note: I used "fetch_openml" method to load MINST dataset, so there is no need to download the dataset and set the path manually for the code to work.**
