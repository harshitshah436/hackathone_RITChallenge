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

###Aproach 1 (Java app using weka .model)
#####Extracting .model file
0. Make a model using any available data mining tool like Weka[http://www.cs.waikato.ac.nz/ml/weka/] or rapid miner[https://rapidminer.com/].
1. Apply classification (data mining) algorithm and classify based on newly added column. I would apply J48 algorithm which is java implementation of c4.5 decision tree algorithm.
2. Export .model file.

#####Java app
0. Now you start developing app using SWING Gui or implement front end using css and js
1. I would implement app using SPRING MVC library or REST Web services because it will be more user friendly to extend in future and easy to implement.
2. Load your .model file using weka java library.
3. Take inputs from user like question, then instead of make user waiting for the reply from us, just give their query to our model and saw them the expected result with high UI and according to their age and interest.

###Aproach 2 (Use text mining and show the results with high UI)
0. I would go for simple k-means clustering algorithm and divide the output into my expected three clusters (Objectives).
1. Then based on this clustering make an app with UI which shows the user a result with high graphics and UI.

####Notes: 
* index.html file is expected form to be designed using css and javascipt. Even we can import it in other jsp if needed.
* model_decision_tree.jpg is just a high level image of what should be expected after applying data mining algorithm on updated raw data. There will be many nodes unlike in the image.
* output_flow.jpg displays how output should be achieved from the reason entered in the form by user
* There will be more classes at the back end depending on the architecture used like SPRING MVC or RESTFul webservices in java.
