# Evaluation and Comparison of Machine Learning Frameworks in Big Data
<h4>Introduction: </h4>
<p> The analysis is limited to evaluating one machine learning algorithm on three different machine learning frameworks. Not all the frameworks available in the market today supports all the machine learning algorithms. These frameworks are designed to handle and work efficiently only for a particular category of algorithms like classification, clustering, deep learning etc. For example, Keras an machine learning framework is primarily built for unsupervised clustering-based algorithms.  We are comparing a classification algorithm against three machine learning toolkits that are used as a part of big data technologies. 
</p>
<h4> Dataset: </h4>
<p> The analysis is limited to evaluating one machine learning algorithm on three different machine learning frameworks. Not all the frameworks available in the market today supports all the machine learning algorithms. These frameworks are designed to handle and work efficiently only for a particular category of algorithms like classification, clustering, deep learning etc. For example, Keras an machine learning framework is primarily built for unsupervised clustering-based algorithms.  We are comparing a classification algorithm against three machine learning toolkits that are used as a part of big data technologies. 
</p>
<h4> Setup:</h4>
<p>The tests have been carried out in the cluster setup done on Microsoft Azure. Azure clusters support many of the machine learning framework that come with pre-configured tools required for executing the code and storing data. Total cluster node-10 with max ram of 28GB, with the following split Head - 8 cores, 2 nodes, Worker – 32 cores, 4 nodes, Edge nodes –8 cores, 1 node.  </p>


<h4>Machine Learning Frameworks: </h4>
<ol>
<li> MLlib </li>
<li> H2O </li>
<li> SparkR </li>
</ol>

<h4> Algorithm used</h4>
 <p>Random Forest</p>

<h4>Conclusion </h4>
<p>The Spark (MLlib) implementation is fast, memory efficient and uses all cores. It deals with categorical variables automatically. For larger datasets (0.1m) it had the lowest time taken to train compared to other tools.  Spark has the least memory footprint.
H2O implementation is slower and has a larger memory footprint. It runs out of memory for 1M dataset. It also has less memory footprints compared to SparkR even for large datasets.
SparkR implementation is comparatively slower than MLlib. It has larger footprints and takes more time to train even for smaller datasets. 
MLlib appears to have better performance for random forest algorithm when compared to the other frameworks. It runs large datasets given the same cluster configuration efficiently. It has the least time taken to train the model for larger datasets. The memory footprints are less compared the other frameworks. It has the highest AUC for the given datasets.
</p>
