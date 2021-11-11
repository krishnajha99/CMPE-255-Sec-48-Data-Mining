# Dimensionality Reduction - Analysis
**Dimensionality Reduction Techniques Tabular and image base Data Set**
Dimensionality reduction is the process of reducing the dimension of the feature set while maintaining its structure and usefulness.Dimensionality reduction features we can use intense  data we need to train for a good model. Expanding on this, if we have a fixed amount of training data  model's accuracy will decrease for every feature you have.

Data 64x64 image we have 4096 features! One way to reduce that number (and hopefully produce a more accurate model) is to effectively compress the image. We do this by trying to find a way of keeping as much information as possible about the image without losing the essential structure.

MNIST Dataset : Using Keras library and CNN (Convolutional Neural Network). The model is 94-95% accurate. While running the hand_detection.py, try to fix your hand in the blue box to get high accuracy.

Tabular Un-standardized data is sensitive to the variances of the initial variables. The variables with larger ranges dominates over those with small ranges (a variable that ranges between 0 and 100 will dominate over a variable that ranges between 0 and 1), which leads to biased results. Transforming the data to comparable scales prevents this problem.

Mathematically, this can be done by subtracting the mean (or emperical mean - sample mean of each column shifted to zero) and dividing by the standard deviation for each value of each variable.

Colab Link for image processing - <a href="https://colab.research.google.com/drive/1FeLvngCUJ9caIlik9vt-r93e1K2d3Zj7?usp=sharing">Google Colab Link</a>

Colab Link for tabular data processing - <a href="https://colab.research.google.com/drive/1Vwg76vp21cA9DSZvZodK215scxRguB7h?usp=sharing">Google Colab Link</a>

Dataset Link - <a href="https://drive.google.com/drive/folders/115WQD1JoWu9TUQibN0k48ElEpk0qxYeb?usp=sharing">Google Drive Link</a>

### **Summary**
