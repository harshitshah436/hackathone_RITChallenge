## hackathone_RITChallenge

####Data Using:
Turbotax Answer Exchange Data. URL [https://www.dropbox.com/s/5bc58el3v3ohwaw/output.csv.zip]

####Objective is to understand tax implications of important life changes, specific to 
* Buying your first home,
* Having your first baby,
* and/or getting married.

####Data must be cleaned before considering it for the app
* The current data has to be cleaned because you can't understand what it is trying to say about tax implications specific to the above objectives
* Remove meaningless columns like create At, Edition, platform, etc..
* Add new column finding out a key word from Reply column regarding to home, baby and married.

###Aproach 1
0. Make a model using any available data mining tool like Weka[http://www.cs.waikato.ac.nz/ml/weka/] or rapid miner[https://rapidminer.com/].
0. Apply classification (data mining) algorithm and classify based on newly added column. I would apply J48 algorithm which is java implementation of c4.5 decision tree algorithm.
0. Export .model file.
1. Now you
