# Unsupervised Learning
In Machine learning, there are basically four types of learning: supervised learning, semi-supervised learning, unsupervised learning
and reinforcement learning.
Dataset in unsupervised learning is collection of unlabeled examples. The goal of an unsupervised learning alogrithm is to create a model that takes a feture vector as input and either transforms it into another vector or into a value that can be used to solve a practical problem. For example, in clustering, the model returns the id of the cluster for each feature vector in the dataset. In dimensinality reduction, the output of the model is a feature vector that has fewer features than the input; in outlier detection, the output is a real number that indicates how input is different from a typical" example in the dataset.

# Summary of References
## An unsupervised learning method for perceived stress level recognition based on office working behavior
* In this paper, the author wants to study the relationship between working behaviors and stress level of people. The author uses the  unsupervised learning on the data set and found the relation of each cluster to a stress level, which was measured by using Perceived Stress Scale (PSS) 
* For data collection, the author use and collect data from Arduino, Raspberry Pi, and multiple sensors. For example, for the working behavior attributes, the force sensor embedded in seat cushion recognizes how often the subject change their posture from sitting to standing. And for enviornment, different sensors like temperature sensor will be connected to Arduino and collect data.
* For unsupervised learning, we could identify the similar working behavior which related to high or low stress more efficiently by using unsupervised learning and cluster analysis, the clustering algorithms we used in this process are k-means clustering and hierarchical clustering algorithm.
* number of instances in each cluster
![](https://github.com/ZhaoPeixi627/miniporject_2/blob/master/Mini_Project_2/Number%20of%20instances%20in%20each%20cluster.png)
* character of two clusters
![](https://github.com/ZhaoPeixi627/miniporject_2/blob/master/Mini_Project_2/character%20of%20two%20cluster.png)
## Unsupervised Deep Transfer Feature Learning for Medical Image Classification
* There is a paucity of annotated data available due to the complexity of manual annotation, so to overcome this problem, we use unsupervised learning alogrithm.
* ropose a new hierarchical unsupervised feature extractor by introducing a zero-bias CAE placed atop of a pre-trained CNN
* Zero-Bias Activation at Encoding-time
![](https://github.com/ZhaoPeixi627/miniporject_2/blob/master/Mini_Project_2/Zero-Bias%20Activation%20at%20Encoding-time.png)


# Analysis of results including pros and cons
Since there is no label for the unsupervised learning, it retains it self-retention to find the structure in its input. Unsupervised learning is a challenging goal in itself. The training data consists of a set of input vectors x without any corresponding target value;
## Pros
1. The potential of hidden patterns can be very powerful for the business or even detect extremely amazing facts, fraud detection etc.
2. K-Means: The algorithm is simple and easy to implement.
3. It can detect what human eyes can not understand
4. Output can determine the un explored territories and new ventures for businesses. Exploratory analytics can be applied to understand the financial, business and operational drivers behind what happened.
## Cons
1. Unsupervised learning is harder as compared to supervised learning.
2. SUpervised learning is more efficient and accurate than unsupervised learning.
3. Usefulness of the results; are of any value or not is difficult to confirm since no answer labels are available.

# Recommendation
In unsupervised learningh, common clustering algorithms include:
1. Hierarchical clustering: In this technique the algorithm builds a multilevel hierarchy of clusters by creating a cluster tree
2. k-Means clustering: Here data gets partitions into k distinct clusters based on distance to the centroid of a cluster
3. Based on density clustering DBSCAN: Density-Based Spatial Clustering of Applications with Noise
4. Gaussian mixture models: Algorithms builds a model in which model clusters a mixture of multivariate normal density components
5. Based on density clustering Mean Shift: Shift mean is compared to k-means, both of which move the center point with the mean of the points within the collection, except that shift mean can determine the number of class clusters
6. Self-organizing maps: This one gets super simplified by using neural networks that learn the topology and distribution of the data
7. demensionality reduction: CPA: It has no parameter limits at all. There is no need for artificially set parameters or intervention in calculations based on any empirical model in the calculation of the PCA, and the final results are only relevant to the data.
8. Hidden Markov models: Simply uses observed data to recover the sequence of states

# Conclusion
Unsupervised learning deals with problems in which data doesn't have labels. That property makes it vert problematic for many application. The absence of labels representing the desired behavior for your model means the absence of a solid reference point to judge the quality of your model. Sometimes people can't judge if the model or label resulted by unsupervised learning is corret or not. There is no error or reward signal to evaluate a potential solution. The number of cluster seekers can be chosen adaptively as a function of the distance between them and the sample variance of each cluster. The best use for unsupervised is around exploratory analytics to understand the financial, business and operational drivers behind what happened.

# Reference
[1] An unsupervised learning method for perceived stress level recognition based on office working behavior. Worawat Lawanont, Masahiro Inoue  Shibaura Institute of Technology, Japan

[2] Unsupervised Deep Transfer Feature Learning for Medical Image Classification. Euijoon Ahn, Ashnil Kumar, Dagan Feng, Michael Fulham and Jinman Kim

[3] The Hundred-Page Machine Learning Book. Andriy Burkov

[4] Unsupervised Learning an Angle for Unlabelled Data World. Vinod Sharma,2018

# Group Members' Report
## Meachine Learning Advancements -- Danny
* Two traditional approaches to language translation. The first one is machine translation. The challenges of machine translation: 1. so many rules for different languages. 2. Natural ambiguity and flexibility of human language. The second approch is called statistical neural translation. This model works particularly well with short phrases but fails on larger texts which cannot be discounted in the translation possibilities. The latest and state of the art in language processing utilizes neural machine translation is called Google NMT. Neural machine translation uses neural networks to learn a statistical model for machine translation. The model can learn on input and output text directly, thus removing the requirements for rules of each of the languages. The cons of this are that languages with extremely high amount of data tend to get worse, more languages added to this universal model, the quicker the quality drops. 

## Machine Learning:Detect and Segment Object -- Xushan
* Tensorflow zoo is a good starter for user to apply different models of machine learning. In my report, I just analysis three models in the zoo: SVM model, mask R-CNN model and R-FCN model. SVM model is a very popular classification method in machine learning, which suitable to be used in the situation of kernel function known. However, it is hard to find the kernel function in the situation of high dimension space, and it need more storage space. Mask R-CNN model is an advanced version of Faster R-CNN model, it has high performance for generating object instance segmentation, however, the process is too slow. The last one is R- FCN, which is a detection model include a ROI pooling layer. It also reflect the spatial location information of the object. R- FCN seems to have the highest accuracy and fast operation speed among these models. In addition, there are a lot of other models in Tensorflow zoo and many datasets which are provided to users.

## CNN -- Yunze
* CNN is a very useful method to detect objects in images is a classical problem in computer vision, but CNN is usually used for detecting one image. R-CNN. R is for region. The region proposals are usually derived in through an algorithm called selective search. A selective search on an image generally provides around 2000 region proposals of interest. Selective search usually use traditional imagine processing technology to find the object.

## Meachine Learning -- Chenhui
* There are numerous approaches that can used in the segment detection. In this project, the DeeplabV3 is the best architecture in terms of segment detection, compared with the former version, the DeeplabV3 not only decreases the speed, but also increase the mIOU significantly. The experimental results show that the proposed model significantly improves over previous DeepLabV3 and achieves comparable performance with other state-of-art models on the PASCAL VOC 2012 semantic image segmentation benchmark. 


