
# State of art libraries for Approximate nearest neighbor search for LightFM data set.
The LightFM's built-in Dataset class to build an interaction dataset from raw data. https://archive.org/details/stackexchange

The goal is to demonstrate how to use different ANN Search works

- LSH
- Exhaustive search
- Product quantization
- Trees and graphs
- HNSW

Data Set Dependencies:

- Annoy <br>
- NMSLIB

Colab Link for ANN - <a href="https://colab.research.google.com/drive/11xKQJy87Q7L8GneDDBz1QHicp7yw0GV2?usp=sharing">Google Colab Link</a>

<b> Summary: </b>
Based on above HNSW(NMSLib) is by far and away the best choice here. Trees and Graphs’s(annoy) performance is the worst at this particular task, it performs much better with cosine based lookup (like when computing similar items). Also, the indices are all memory mapped from file, which makes it much more suitable if you have multiple python processes serving up requests.
