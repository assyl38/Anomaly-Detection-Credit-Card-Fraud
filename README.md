# Anomaly-Detection-Credit-Card-Fraud
## What is anomaly detection
Anomaly detection is the identification of rare events, items, or observations which are suspicious because they differ significantly from standard behaviors or patterns. Anomalies in data are also called standard deviations, outliers, noise, novelties, and exceptions.
</br>
In the network anomaly detection/network intrusion and abuse detection context, interesting events are often not rare—just unusual. For example, unexpected jumps in activity are typically notable, although such a spurt in activity may fall outside many traditional statistical anomaly detection techniques.
</br>

Many outlier detection methods, especially unsupervised techniques, do not detect this kind of sudden jump in activity as an outlier or rare object. However, these types of micro clusters can often be identified more readily by a cluster analysis algorithm.
</br>

There are three main classes of anomaly detection techniques: unsupervised, semi-supervised, and supervised. Essentially, the correct anomaly detection method depends on the available labels in the dataset.
</br>

Supervised anomaly detection techniques demand a data set with a complete set of “normal” and “abnormal” labels for a classification algorithm to work with. This kind of technique also involves training the classifier. This is similar to traditional pattern recognition, except that with outlier detection there is a naturally strong imbalance between the classes. Not all statistical classification algorithms are well-suited for the inherently unbalanced nature of anomaly detection.
</br>

Semi-supervised anomaly detection techniques use a normal, labeled training data set to construct a model representing normal behavior. They then use that model to detect anomalies by testing how likely the model is to generate any one instance encountered.
</br>

Unsupervised methods of anomaly detection detect anomalies in an unlabeled test set of data based solely on the intrinsic properties of that data. The working assumption is that, as in most cases, the large majority of the instances in the data set will be normal. The anomaly detection algorithm will then detect instances that appear to fit with the rest of the data set least congruently.

<p align='center'>
<img width="800" height="200" src="https://avinetworks.com/wp-content/uploads/2017/04/anomaly-detection.png"> </br>
<em> Anomaly Detection FAQs
 </em>
</p> 

## Anomaly detection techniques

In searching data for anomalies that are relatively rare, it is inevitable that the user will encounter relatively high levels of noise that could be similar to abnormal behavior. This is because the line between abnormal and normal behavior is typically imprecise, and may change often as malicious attackers adapt their strategies.
</br>

Furthermore, because many data patterns are based on time and seasonality, there is additional baked-in complexity to anomaly detection techniques. The need to break down multiple trends over time, for example, demands more sophisticated methods to identify actual changes in seasonality versus noise or anomalous data.
</br>

For all of these reasons, there are various anomaly detection techniques. Depending on the circumstances, one might be better than others for a particular user or data set. A generative approach creates a model based solely on examples of normal data from training and then evaluates each test case to see how well it fits the model. In contrast, a discriminative approach attempts to distinguish between normal and abnormal data classes. Both kinds of data are used to train systems in discriminative approaches.
</br>

### Clustering-Based Anomaly Detection
Clustering-based anomaly detection remains popular in unsupervised learning. It rests upon the assumption that similar data points tend to cluster together in groups, as determined by their proximity to local centroids.
</br>
K-means, a commonly-used clustering algorithm, creates ‘k’ similar clusters of data points. Users can then set systems to mark data instances that fall outside of these groups as data anomalies. As an unsupervised technique, clustering does not require any data labeling.
</br>

Clustering algorithms might be deployed to capture an anomalous class of data. The algorithm has already created many data clusters on the training set in order to calculate the threshold for an anomalous event. It can then use this rule to create new clusters, presumably capturing new anomalous data.
</br>
However, clustering does not always work for time series data. This is because the data depicts evolution over time, yet the technique produces a fixed set of clusters.


## Density-Based Anomaly Detection

Density-based anomaly detection techniques demand labeled data. These anomaly detection methods rest upon the assumption that normal data points tend to occur in a dense neighborhood, while anomalies pop up far away and sparsely.
</br>

There are two types of algorithms for this type of data anomaly evaluation:
</br>
- K-nearest neighbor (k-NN) is a basic, non-parametric, supervised machine learning technique that can be used to either regress or classify data based on distance metrics such as Euclidean, Hamming, Manhattan, or Minkowski distance.

- Local outlier factor (LOF), also called the relative density of data, is based on reachability distance.

- Support Vector Machine-Based Anomaly Detection
</br>


A support vector machine (SVM) is typically used in supervised settings, but SVM extensions can also be used to identify anomalies for some unlabeled data. A SVM is a neural network that is well-suited for classifying linearly separable binary patterns—obviously the better the separation is, the clearer the results.
</br>
Such anomaly detection algorithms may learn a softer boundary depending on the goals to cluster the data instances and identify the abnormalities properly. Depending on the situation, an anomaly detector like this might output numeric scalar values for various uses.

# Credits
[Anomaly Detection ](https://avinetworks.com/glossary/anomaly-detection/#:~:text=Anomaly%20detection%2C%20also%20called%20outlier,differ%20significantly%20from%20the%20norm.)  </br>
[Anomaly Detection Kaggle](https://www.kaggle.com/code/naveengowda16/anomaly-detection-credit-card-fraud-analysis/notebook)
