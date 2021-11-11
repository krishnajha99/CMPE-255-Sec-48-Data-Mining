# Dimensionality Reduction - Analysis (Tabular and image Data Set)
Dimensionality reduction is the process of reducing the dimension of the feature set while maintaining its structure and usefulness. Dimensionality reduction features we can use intense data we need to train for a good model. Expanding on this, if we have a fixed amount of training data, the model's accuracy will decrease for every feature you have.

Data 64x64 image we have 4096 features! One way to reduce that number (and hopefully produce a more accurate model) is to effectively compress the image. We do this by trying to find a way of keeping as much information as possible about the image without losing the essential structure.

MNIST Dataset : Using Keras library and CNN (Convolutional Neural Network). The model is 94-95% accurate. While running the hand_detection.py, try to fix your hand in the blue box to get high accuracy.

Tabular Un-standardized data is sensitive to the variances of the initial variables. The variables with larger ranges dominate over those with small ranges (a variable that ranges between 0 and 100 will dominate over a variable that ranges between 0 and 1), which leads to biased results. Transforming the data to comparable scales prevents this problem.

Mathematically, this can be done by subtracting the mean (or empirical mean - sample mean of each column shifted to zero) and dividing by the standard deviation for each value of each variable.

In the below Colabs demonstration for the Image and tabular dataset for various techniques used Dimensionality Reduction.

Colab Link for image processing - <a href="https://colab.research.google.com/drive/1FeLvngCUJ9caIlik9vt-r93e1K2d3Zj7?usp=sharing">Google Colab Link</a>

Colab Link for tabular data processing - <a href="https://colab.research.google.com/drive/1Vwg76vp21cA9DSZvZodK215scxRguB7h?usp=sharing">Google Colab Link</a>

Dataset Link - <a href="https://drive.google.com/drive/folders/115WQD1JoWu9TUQibN0k48ElEpk0qxYeb?usp=sharing">Google Drive Link</a>

Analysis:-

- Both the Colab use cases less time in training the dataset.
- Easy visualization of the dataset containing 2 or 3 principle features in both the dataset.
- Results showing the higher performance.

Manifold Learning based focus for the both dataset
In many cases where the subspace may twist and turn(Swiss roll), projection is not the best approach to dimensionality reduction. Manifold Learning techniques measures how each training instance linearly relates to its closest neighbors, then it looks for a low-dimensional representation of the training set where these local relationships are best preserved.

Steps To Perform PCA:

1. Standardize The Data: 
Data Should Be Standardized While Performing PCA. Therefore, Standardisation Will Be Done By Subtracting The Mean And  Dividing By Standard Deviation. After Standardization Data Comes Into The Same Scale.
Z=Value-Mean/Standard Deviation               

2. Calculate The Covariance Matrix 

3. Dimensional Data, Covariance Matrix Will Be Represented As 

Covariance Matrix For 3-Dimensional Data
Covariance Matrix For 3-Dimensional Data
Covariance: Measures The  Correlation Between X And Y

• When Cov(X,Y)=0: Independent

• Move In Parallel Direction : If Covariance (X,Y)>0

• Cov(X,Y)<0: Move Opposite Direction

4. Extraction: 
In Feature Extraction ,Creating New Features Reduces High Dimensional Features To Fewer Dimensions. Features  Having Similar Properties Are Combine And Form One Group. So, This Will Help In Reducing The Number Of Features And Make It Easy For Models To Perform Better. 

There Are Many Feature Extraction Technique the below six  dimensionality reduction techniques for data visualization : (PCA, t-SNE, UMAP, LLE, ISOMAP, SVD)and tried to use them to visualize a high-dimensional dataset in 2d and 3d plots.

PCA-Principal Component Analysis 
T-SNE-(T-DistributedStochastic Neighbor Embedding
SVD-Singular Value Decomposition
UMAP-Uniform Manifold Approximation and Projection
LLE-Locally Linear Embedding
ISOMAP-Isometric mapping methods, and extends metric multidimensional scaling

### **Summary**
Dealing with thousands and millions of features is a must-have skill for any data scientist. The amount of data we are generating each day is unprecedented and we need to find different ways to figure out how to use it. Dimensionality reduction is a very useful way to do this and has worked wonders for me, both in a professional setting as well as in machine learning process. Also dimensionality reduction may not work very well in all situations. In such cases we need to think out of the box to transform the data into lower dimensional space, also it is important to work with different new reduction algorithms on the same data.
Hope this dimensionality reduction shows real world scenario’s in both the cases.


