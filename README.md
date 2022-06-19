# Supersense-App-
# SISE2601 Project data description
================

Team F

The dataset of the Supersense application contains 24 hours record of users' app usage from 05/10/2021 to 31/10/2021.
The data in this dataset can be divided into four groups of information. The first one is the time category which contains
the date and time the user uses the app. The second category is the location. This category assembles from the geographic
(continent, country, city, …). The third category is all about the events, the type of the event, the object the user 
searched for, and the object the app found, and the last category is about the satisfaction of the user from the app 
(Yes, No, not sure). Our researchfocuses on the app usage and the effect of the usage on the satisfaction with the app;
therefore, this dataset contains the information needed to analyze and answer our research questions. If we look at 
the data, we can see two main entities with a lot of features. The features we will focus on the most are the Event
type and its connection to the user and the useful feature.


| variable | type | description | 
| -------- | ---- | ---------- | 
| event_date| int | The date when the event occur |
| event_timestamp | double | Event time stamp |
| event_name | char | Event name |
| user_pseudo_id | char | The user id value|
| category | char | The category of the application usage, mostly mobile |
| mobile_brand_name | char | The mobile brand name |
| mobile_model_name | char | The model name of the mobile |
| operating_system | char | Operating system type |
| operating_system_version | char | Operating system version |
| language  | char | The language that the user used in the app|
| continent | char | The continent where the user used the app |
| country | char | The country where the user used the app |
| region | char | The region where the user used the app |
| city | char | The city where the user used the app |
| sub_continent | char | The sub continent where the user used the app |
| value  | Char | Indicate the the explore feature started (explore.csv)|
| session_id | int | The session id number,(seasson.csv) |
| object_name | char | The objec |
|



Kmean Model instructions:
1.Run all the cells that importing the data from the csv files
2.Run the joining cell (named func_data2)
3.Run the Kmeans model with different K value
4.Draw the graph of the K,TOTTS
5.After analyzing the graph, pick the best K according to the elbow method.
6.Get the summary of the kmean model with the best k
7.Visualize the Kmean partition.

To run the Kmean model first we gathered from all the csv files related to the app features and count the number of featured used for each feature and each user. Then we joined all the data into one data frame. We run the Kmean model over searval k values and pick the best k for our data.Then using summary over the Kmean results and visualize the Kmeans groups we analyized the results.


Decision tree model instructions:
1. Import the find_useful.csv.
2. Join the find_useful data with func_data2.
3. Filter the table to the specific column ("num_of_read_uses","num_of_find_uses","num_of_explore_uses","answer").
4. Run the Decision tree model on the data.
5. Visualize the Decision tree model.
6. Creating the confition matrix.
