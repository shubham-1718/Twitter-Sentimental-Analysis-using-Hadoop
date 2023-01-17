# Twitter Data Analysis
In this Project I am going to analyze the data from twitter i would collect the data from twitter and do a sentimental analysis. I have used Java Language code to write Map-reduce job, Flume for data collection and HiveQL to analyze and generate report.

Sentiment analysis is the analysis of people’s opinions, sentiments, evaluations, appraisals, attitudes and
emotions in relation to entities like individuals, products, events, services, organizations and topics by
classifying the expressions as negative / positive opinions.

In this project you i be trying to do sentiment analysis of the opinions on twitter using Hadoop Eco-
System. The reason i chose twitter is because the social media is gaining popularity for the customer
reviews and it is also creating a good business-customer relationship in the market. The reviews would
certainly reflect the service of the company in the market.

Objectives:

The objective of the project is to find the sentiments of the users on Twitter. Companies can analyze the
sentiments of the users regarding their products / services and use it for betterment of the same.

Plan of work:

Collect Data: The initial step is to collect all twitter tweets.
Pre-process Data: I need to write MR job to pre-process the data
Classification of Data: Write Hive UDF for the classification of the data into positive / negative
opinions
Print Data: Final stage would be to print the desired results with the number of good and bad
tweets collected.

Architecture: I have followed below architecture to analyze the data from twitter and generated report.                     


    [user](user tweets about his opinion or feedback on twitter) ---------> [Twitter] (Twitter stores tweets in Json format) ---------->[Apache Flume Server](Flume uses twitter4j API to connect to the twitter streaming API which gives constant stream of tweets. from here flume will start writing data into HDFS) ---pre-processing is done by mapreduce------> [Hadoop Cluster] ----------->[Hive](used hive UDF for classification and queries for reporting) ------------>[Report Generated from hive output]
    
Please Read [Assignment steps.txt] to understand the workflow.
