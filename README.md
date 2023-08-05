# PySpark

Customer churn is a critical challenge faced by banks and financial institutions, leading to significant revenue loss and reduced business growth. This project aims to address this issue by utilizing Apache Spark, a powerful distributed computing framework, to analyze bank customer data. By building a churn prediction model, we seek to identify customers at risk of churning and provide insights that can guide effective customer retention strategies, ultimately improving the institution's overall performance and customer satisfaction.

Installation
--
**1. Install Java Development Kit (JDK)**

Spark requires Java to be installed on your system. Download and install the latest version of JDK from the Oracle website or any other official source.

**2. Download Spark**

Visit the Apache Spark website (https://spark.apache.org/) and download the latest version of Spark. Unzip the downloaded file to a preferred location on your computer.

**3. Set Environment Variables**

Set the following environment variables in your system:

**JAVA_HOME:** *Point it to the directory where Java is installed.*

**SPARK_HOME:** *Point it to the Spark installation directory.*

**PATH:** *Add %SPARK_HOME%\bin and %SPARK_HOME%\sbin to the PATH variable.*

**4. Install FindSpark**

FindSpark is a Python library that allows Jupyter Notebook to locate Spark installed on your system. Install it using pip:

``
pip install findspark
``

**5. Configure Jupyter Notebook**

Make sure you have Jupyter Notebook installed. If not, install it using:

`` 
pip install jupyter 
``

**6. Start Jupyter Notebook**

Launch Jupyter Notebook by running the following command in your terminal:

`` 
jupyter notebook 
``

A web browser will open with the Jupyter interface.

**7. Connect Jupyter Notebook to Spark**

In your Jupyter Notebook, create a new notebook and add the following code to connect it to Spark:

```
import findspark
findspark.init()
from pyspark.sql import SparkSession

spark = SparkSession.builder.appName("ChurnAnalysis").getOrCreate()
```

You are now ready to use Spark within Jupyter Notebook for churn analysis!

Dataset
--
The contains various features related to bank customers, such as age, balance, number of products, tenure, and other relevant attributes. The target variable is the "churn" column, indicating whether a customer has churned (1) or not (0). The dataset is available [here.](https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset)

Related Sources
--
If you want to learn more about big data technologies you can read my medium article [here.](https://medium.com/@miraytopal/b%C3%BCy%C3%BCk-veri%CC%87ni%CC%87n-i%CC%87ki%CC%87-devi%CC%87-hadoop-ve-spark-457ea8d83a39)


License
This project is licensed under the [Apache License 2.0](https://github.com/miraytopal/PySpark/blob/main/LICENSE) License. Feel free to use and modify the code as per the license terms.

Contributions to this repository are welcome! If you have any ideas for improvements, feel free to create a pull request.✨💪
