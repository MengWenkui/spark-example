spark-example
=============

A small example illustrating Logistic Regression on Spark


Getting the Data 
----------------

You can get the data set from this URL: [https://archive.ics.uci.edu/ml/datasets/banknote+authentication]
(Click on Data Folder)


Dependencies
--------------

You need to have:

    Python >= 2.7  (not 3.x)
    Numpy >= 1.7
    Hadoop (Optional)
    Spark (If you want to run with Hadoop, then it needs to be compiled to that Hadoop version)

Running the Example
----------------
You need to have Spark Installed and Compiled. 
After that running the example includes changing a few variables in the Python file:

    SPARK_HOME = "/usr/local/spark-0.9.1" # Set this to wherever you have compiled Spark

and

    data = sc.textFile("hdfs://localhost/user/hduser2/data") # change the path to wherever you have put the dataset file


To Run:

    python run-spark-ex.py
    
Last line will be the training error:

    Training Error = 0.0211370262391
