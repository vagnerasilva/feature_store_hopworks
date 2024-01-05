# feature_store_hopworks


# 1
https://research.aimultiple.com/feature-store/#:~:text=Feature%20stores%20help%20data%20science,be%20utilized%20by%20various%20models.
What are the advantages of a feature store?
Feature stores enable businesses and data science teams to:

Save time through advanced feature reusability
Creating features is a time-consuming process that requires domain expertise about the problem. Feature stores help data science teams store the features that are created for a problem and reuse them for another problem. For example, the processed data about the average shipping time of a company or the standard delivery time of a restaurant can be utilized by various models. Reusability of features helps ML teams to accelerate the ML model development process.

# 2
https://towardsdatascience.com/the-importance-of-having-a-feature-store-e2a9cfa5619f
Why do we need feature stores?

There are a few feature-specific challenges data scientists face that the use of feature stores helps alleviate. These include:

Features are not reused. A common obstacle data scientists face is spending time redeveloping features when using previously developed features or ones developed by other teams would have sufficed. Feature stores allow data scientists to avoid repeat work.
Feature definitions vary. Different teams at any one company might define and name features differently. Moreover, accessing the documentation of a specific feature (if it exists at all) is often challenging. Feature stores address this issue by keeping features and their definitions organized and consistent. The documentation of the feature store helps you create a standardized language around all of the features across the company. You know exactly how every feature is computed and what information it represents.
There is inconsistency between training and production features. Production and research environments often use different technologies and programming languages. The data streaming in to the production system needs to be processed into features in real time and fed into a machine learning model. For the modelling effort to be effective, the model developed offline in research needs to provide the exact same prediction as the model deployed online given the same data as input. Having a feature store that is environment agnostic (online and offline) suggests that given the same data, the model will be fed the same feature exactly.‍

# 3
https://h2o.ai/blog/2022/what-are-feature-stores-and-why-are-they-important/
There you have it, a whirlwind tour of feature stores and some of their most significant benefits. Their use is spreading, but it is by no means an industry standard. Indeed, the FANG companies built their own from scratch! The fact they are investing heavily in this technology should demonstrate that it is here to stay and is an essential component if you want to perform top-notch machine learning at scale.

Implementing a feature store now will likely give you a competitive advantage. Expect significant productivity gains, deeper company-wide data understanding, and more models to be put into production faster. If you want to implement a cutting-edge feature store to transform your business, sign up  for early access today.

# 4
https://deepchecks.com/why-are-feature-stores-important/
Importance of Feature Stores
Features are hosted at multiple places by different teams in an enterprise. Feature stores provide a centralized feature storage option.
Feature stores also help transform the features suitable for the production environment eliminating the need for extensive data engineering.
Feature stores promote feature reusability and sharing of features consistently throughout the organization amongst different teams.
Feature stores also monitor the correctness of the feature pipelines in production environments.
Feature stores also provide feature definition consistency, feature versioning, and metadata.


# 5
https://www.linkedin.com/pulse/how-feature-store-can-supercharge-your-productivity-data-kingre/


# 6
https://www.teraflow.ai/ml-feature-stores-why-you-need-a-feature-store/
Feature stores provide a number of benefits that can save organisations both time and money.

Dominic Kafka: “Especially around computing costs. When data is dispersed across different locations or formats, it can be difficult and expensive to compute. A feature store helps to consolidate all that data into a manageable format, making things easier and more affordable.”

They make data more accessible. Data analysts and scientists need to be able to quickly access the data they need in order to build models and analyse results. A feature store simplifies this process by providing an easily accessible location for all data-related features. This includes data that is stored in different formats or locations.

# 7 
https://opendatascience.com/the-rising-importance-of-feature-stores/
Common Problems Feature Stores Can Solve

Every data science project begins with a qualified search for the right features to be consumed by the algorithm. The problem is there typically isn’t a single, central location to search; features are hosted in many places, especially in a large enterprise. The solution offered by a feature store is that it provides a principal repository for sharing all available features. When a data scientist starts a new project, he or she can go to this collection and easily find the required features. A feature store is also a data transformation service enabling data scientists to handle raw data and store it as features ready to be used by a machine learning model.

Feature stores aim to solve the full complement of data management challenges encountered when building and operationalizing machine learning applications. Here is a short-list of a number of enterprise machine learning issues that feature stores can help resolve: 

Productionize features without extensive support from data engineering 
Automate feature computation via transformations
Share and reuse features across pipelines for various teams
Provide feature versioning, lineage, regulatory compliance, and metadata
Attain consistency between training and inferencing
Monitor the condition of feature pipelines in production environments

# 8 
https://www.linkedin.com/pulse/do-you-really-need-feature-store-gantry-ml/
Why you probably don’t need a feature store
If you’re building out your ML stack, you’ve probably considered implementing a feature store. Used by companies like Uber, Netflix, Airbnb and Google, a feature store is often presented as a necessary part of production ML.
But, this article asks whether you really need a feature store - and their answer is ‘no’. At least, not unless there are some specific circumstances that justify the additional complexity that using one will create.
This article sets out what those circumstances are, and the alternative approaches that could serve your needs just as well.

# 9
https://pub.towardsai.net/unleashing-the-power-of-feature-stores-how-they-can-supercharge-your-mlops-30105fb7d3b8
Re-usability of features across various applications
One of the challenges that data science teams often face is duplicated efforts in feature engineering. This occurs when there is no centralized place to manage and fetch features, which results in teams working in silos and reusing features not being straightforward. Additionally, there is an overhead cost associated with using many features. However, using a feature store can help alleviate these challenges by allowing teams to easily share and reuse features across different applications.

# 10
https://blog.dataiku.com/reuse-at-its-best-the-benefits-of-feature-stores
Do You Need to Look at Feature Stores for Your Organization?
There are two main reasons that drive many organizations to look at feature stores:

To limit duplication of work  
To reduce the risk of training/serving skew 
Duplication of work happens when a data scientist develops a feature that was already built by another data scientist for a previous project instead of reusing the existing work. In a credit card company, a feature computing the number of transactions on a card in the previous three months can be beneficial to multiple use cases, such as in both a fraud prediction model and in a customer churn model. Without the proper processes and tooling to provide visibility into the existing models and features, it is very hard to avoid this problem. 

Training/serving skew happens when the feature generation code in the serving pipeline behaves differently than in the model training pipeline. These differences in code behavior can lead to different feature distributions in the records to score compared to the records that were used to train the model, which ultimately leads to poor model performance in production. 

In some organizations, data scientists write feature generation code to train models in Python and hand it over to engineers that reimplement the code — sometimes in another language like Java or C# — for scoring in production. This reimplementation step is both time consuming and error prone. A small difference in code logic can change model input values and impact the model performance in production.This is another example of duplication of work between the data scientist and engineer, which can also curb the ability to run quick iteration cycles on the models.
