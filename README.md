## Detecting patterns from large datasets
### Clustering algorithms :
These algorithms are helpful for analysing large amount of unstructured data such as texts collected from different sources. Clusters can help identify differnt groups, post which each group can be analysed with differnt and more precise techniques according to use case

1. K-Means  _(used in the notebook)_ : Find the optimal centroids and then assigns data points to them
2. KNN : This algorithm only runs at test time, and assigns new data point to a particular class based on it nearest neighbours and the categories they belong to.
3. EM Clustering : This is a soft clustering algorithm, which means points can belong to more than 1 clusters simultaneously.

### Classification and Regression Algorithms :
These algorithms can be used when data is present in more structured format such as sensor data or prices of particular commodity. 
Classification : Used to classify data points to a particular class
Regression : Used to predict a continuous value

1. Random Forest : These models can be used for both classification and regression on structured data. They work well and are resistent to overfitting
2. Naive Bayes Algorithm : Used for classification. Its a simple algorithm with a very fast runtime
3. Boosting Algorithms like XGBoost : Industry standard algorithm for classification/regression. They can be applied to vast variety of datasets and generally perform the best, on given resources
4. Deep Learning : These algorithms perform well but required long training times and large dataset/fine tuning on pretrained models.
  1. Computer Vision : CNN algorithms perform the best
  2. NLP : Transformer algorithms such as GPT

## Possible Approach to follow for real world problems involving large amounts of data from differnt sources
1. Using data pipeline gather data from multiple sources and preprocess it
2. The data can then be broken down into particular segments using clustering algorithms
3. Each segment can individually be analysed and possible converting into structured data (_using NER techniques used in notebook_)
4. Supervised ML algorithms can then be applied to get deeper insights, which might have not been possible earlier since data was too spread out.

### Ethical and Regulatory compliance 
The entire stack(except GPT integration) described in the project uses open source well known techniques and algorithms. 
This allows us to run it on-premises in a completely isolated environment, complying with all regulations.
GPT can also be replaced by open source models such as LLaMa models, which will perform well in this case since the problems the model is solving are more narrow in scope, and the performance can further be improved by fine tuning.

## Working Demo (refer to [notebook](https://github.com/yrao1000/PoliticalManifest-NLP/blob/main/notebook.ipynb) in this repo)
Analysis of Political Manifesto using NLP
