Note: We pivoted in our creative estension idea. Below you will find our updated proposal as well as the old proposal. 

## Milestone P3: Creative Extension Proposal (Updated Proposal)

### 1. Title
* Local and Global prediction of edges and triads in Social Signed Networks???
* Edge prediction in Social Signed Networks????


### 2. Abstract
The research paper aims towards understanding to what extent network theories from social psychology, namely balance and status theory, can be observed in signed network data using 3 different data sets and further how edge predictions can be made with them. With our proposal we want to create a binary weight prediction algorithm based on the triadic structures using balance theory and contrast this approach with another classification method that we name "Average Edge", which is not based on the triadic of the network. We want to try and understand how these two techniques differ from each other in terms of successfull predictions, parameter optimization, and how the resulting predicted edge weights affect the overall triadic structure of new network. Since we want to try to answer additional research questions we will be using the datasets from the original research paper. 

### 3. Research questions

* How do we develop the afore-mentioned prediction techniques.
* To what extent can they be optimized by parameter tuning.
* How do they contrast in terms of performance: accuracy, precision, recall, etc.
* Are we able to draw comparisons between our results and the results found in the research paper?

### 4. Proposed datasets
*  “Epinions”
*  “Slashdot”
*  “Wikipedia”

### 5. Methods
We will replicate the tables from the research paper in order to contrast the results from the different data sets. In addition, we have to try different pre-processing approaches depending on the raw format of the data sets. For example the data set “Bitcoin OTC trust weighted signed network” uses weighted signs, with values ranging from -10 to +10 and therefore we will have to try out different interpretations of "postitive" and "negative sentiment". In addition, since we also have temporal data we will want to analyse how our results change with respect to time and therefore we will make use of time series methods. Concerning, the sentiment analysis we will use natural language processing tools such as "Word2Vec" to determine the degree of postive and negative sentiment of each vote, thereby allowing us to investigate how non-discrete weighted signs affect our results.

### 6. Contributions of Group Members

* Paul: Developed "Average Edge" classification method
* Alexandre: Developed "Balance Theory" classification method
* Arman: Writing up the report and preparing the final presentation.









## Milestone P3: Creative Extension Proposal (Old Version)


### 1. Title
* Generalizing signed network theory: extending research to more datasets and features

### 2. Abstract
The research paper aims towards understanding to what extent network theories from social psychology, namely balance and status theory, can be observed in signed network data using 3 different data sets. With our project proposal we want to extend the analysis to more datasets and verify if we can find similar results pertaining to the latter theories on these new data sets. We are interested in understanding if and to what extent the theories studied in the research paper can be transferred in a more general sense to data with new characteristics. Furthermore, we are interested in seeing how new features such as timestamps and non-binary sign weights affect the interpretation of analyses and conclusions. For our proposal we want to perform the same computational steps as in the paper to then contrast both results, interpret observed differences, and test the limits of social psychology theory for signed network applications. 

### 3. Research questions
* Can balance and status theory be observed in other network data sets?
* Can we explain similarities and differences in results between different data sets?
* How may new data features affect our analysis and results?
* How do our conclusions change with respect to time (temporal data)?

### 4. Proposed datasets
*  “Social Network: Reddit Hyperlink Network” - This data set contains information about links in Reddit, with a network whose edges are connections between subreddits. The network is temporal and directed, with a sign (-1 or 1) for each edge, representing the sentiment of one community toward the target community about posts that create hyperlinks between communities. The sign is the result of a training based classifier on the post, and gives value 1 if the post is considered neutral or positive, and -1 otherwise.
*  “Bitcoin OTC trust weighted signed network” - This data set originates from a "who-trusts-whom" network, where users' reputation is recorded. This is crucial due to the anynonmous nature of bitcoin transactions. On the website Bitcoin OTC users rank each other on a scale from -10 (most distrust) to +10 (most trust) in increments of 1. This signed network data is directed as well as temporal, meaning that a timestamp is provided at each incident of rating.
*  “Wikipedia Requests for Adminship (with text)” - This data set contains information on how users vote for other users who have been requested to become administrators on Wikipedia. A member may select a supporting (+1), neutral (0), or opposing vote (-1). The data creates a directed and signed network and also has the added feature of a textual component that comes with data set, which is a short comment about the candidate written by the voting member that comes with each casted vote. For additional feature processing we can use sentiment analysis and could thus scale the sign of each vote to a number between -1 and +1 instead of having the absolute integer values.

### 5. Methods
We will replicate the tables from the research paper in order to contrast the results from the different data sets. In addition, we have to try different pre-processing approaches depending on the raw format of the data sets. For example the data set “Bitcoin OTC trust weighted signed network” uses weighted signs, with values ranging from -10 to +10 and therefore we will have to try out different interpretations of "postitive" and "negative sentiment". In addition, since we also have temporal data we will want to analyse how our results change with respect to time and therefore we will make use of time series methods. Concerning, the sentiment analysis we will use natural language processing tools such as "Word2Vec" to determine the degree of postive and negative sentiment of each vote, thereby allowing us to investigate how non-discrete weighted signs affect our results.

### 6. Proposed timeline and organization within team
* Every team member will focus on working with one dataset
* Until 4.12: Finish with undirected signed network analysis (balance theory)
* Until 11.12: Finish with directed signed network analysis (status theory)
* Until 15.12: Interpret results and compare with research paper
* 18.12: P4 due date