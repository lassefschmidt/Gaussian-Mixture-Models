# Gaussian-Mixture-Models
Mathematical Intuition and Implementation of Gaussian Mixture Models (unsupervised clustering algorithm)

### Overview of different methods

In Machine Learning, we can generally distinguish between three kinds of learning algorithms:
1. Supervised Learning
2. Unsupervised Learning
3. Reinforcement Learning

In **supervised learning**, we have access to both data and ground truth. For example, given information about houses [such as property size, number of rooms, etc.] and their past sale prices, we could infer future sale prices of other houses. Typical problems include classification and regression.

In **unsupervised learning**, we only have access to the data, but not to the ground truths. In this setting, we wish to discover hidden patterns in our data without human intervention. For example, a firm might have thousands of customers and it struggles to identify a meaningful way to group the customers in different segments (e.g. for a marketing campaign). Typical problems include dimensionality reduction (PCA, NMF, t-SNE, ...) and clustering (kMeans, HDBSCAN, Mixture Models, ...).

Lastly, in **reinforcement learning** we want to build models that can perform sequential decision making with the goal of maximizing some sort of cumulative reward. For example, reinforcement learning was used to finetune the recently released ChatGPT chatbot by OpenAI.

### Goal of this repository

In this repository, we will implement one unsupervised learning algorithm from scratch - namely Gaussian Mixture Models. It can be viewed as the unsupervised version of QDA (Quadratic Discriminant Analysis) or as a generalized version of kMeans (each cluster has its own covariance matrix and we have access to information about the latent centers). In this method, data points are clustered based on their likelihood to belong to a particular distribution. 
