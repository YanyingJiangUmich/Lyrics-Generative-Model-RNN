# The Lyrical Empiricals - Capstone Project
Authors: Yanying Jiang, Josh Horner, Kenny Tang


### Dataset
We obtained our dataset from Kaggle (https://www.kaggle.com/datasets/neisse/scrapped-lyrics-from-6-genres?select=artists-data.csv)
The dataset originally had over 150,000 songs across 4,168 unique artists.
The dataset includes song name, artist name, genres, and lyrics.
For our project, however, we decided to use songs covering 32 American artists with the most songs. After filtering to these artists, we have a little over 1400 songs across 32 artists, each with 300 or more songs.

### How to run our code:
A. Data Cleaning - 
Once the Data has been downloaded, save the data set containing the lyrics as 'lyrics-data.csv'. Then run 'Data Cleaning.ipynb' to obtain 'clean_lyrics_df.csv'. 
In addition, we provided the clean version of the data set in our repository.

B. Exploration - 
After running the Data Cleaning notebook, place the output file (lyrics_clean_df.csv) into the root directory. Make sure the original Kaggle file artists-data.csv is also in the root directory. Then run 'Exploration.ipynb'

C. Clustering - 
Make sure lyrics_clean.csv and artists-data.csv are present in the root directory. Then run 'Genre Clusters.ipynb'

D. Topic Modeling -
There are two separate notebook. One is for the LDA model and the other is for NMF model. They are independent of each other

E. Generative Model 

There are 4 notebooks in the Generative_Model folder: https://github.com/kennyta0204/Capstone-Project/tree/main/Generative_Model
Run them in order 

If encounter errors for Tensorboard, run this in a separate terminal
```
tensorboard --host 0.0.0.0 --logdir=./logs
```


(--host 0.0.0.0: Specifies the host IP address. Setting the host to 0.0.0.0 allows the TensorBoard server to accept connections from any IP address. This is useful when you want to access TensorBoard remotely.

--logdir=./logs: Specifies the directory where TensorBoard will look for your saved files (logs) generated during TensorFlow runs. In the code above, it looks for logs in the logs directory located in the current working directory ./)

You can access the board on URL: http://localhost:6006/ 


