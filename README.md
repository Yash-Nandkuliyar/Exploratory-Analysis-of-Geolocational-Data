# Exploratory-Analysis-of-Geolocational-Data
This project involves the use of K-Means Clustering to find the best accommodation for students in Bangalore (or any other city of your choice) by classifying accommodation for incoming students on the basis of their preferences on amenities, budget and proximity to the location.
Introduction
Implementing the project will take you through the daily life of a data science engineer from data preparation on real-life datasets tovisualizing the data and running machinelearning algorithms, to presenting the results.
In the fast-moving, effort-intense environment that the average person inhabits, it’s afrequent occurrence that one is too tired to fix oneself a home-cooked meal. And of course,even if one gets home-cooked meals every day, it is not unusual to want to go out for agoodmeal every once in a while, for social/recreational purposes. Either way, it’s a commonlyunderstood idea that regardless of where one lives, the food one eats is an important aspect
of the lifestyle, one leads.
Now, imagine a scenario where a person has moved into a new location. They alreadyhave certain preferences, and certain tastes. It would save both the student and the foodproviders a lot of hassle if the student lived close to their preferred outlets. Convenience
means better sales, and saved time for the customer.
Food delivery apps aside, managers of restaurant chains and hotels can also leverage thisinformation. For example, if a manager of a restaurant already knows the demographic ofhis current customers, they’d ideally want to open at a location where this demographic isat its highest concentration, ensuring short commute times to the location and morecustomers served.If potential hotel locations are being evaluated, a site that caters to a widevariety of tastes would be ideal, since one would want every guest to have something totheir liking.
This project is a good start for beginners and a refresher for professionals who havedabbled in python / ML before. The methodology can be applied to any location of one's
choosing, so feel free to innovate!







Literature Survey
[1] This project involves recommending hotels, restaurants and other needs for the user who has accommodated to a area newly. It is difficult for a user to find all the places in a newly accommodated area. So, it is easy if we recommend nearby places. One is too tired to fix oneself a home cooked meal frequently. Even if a person gets home cooked meal every day, it is not unusual to want to go out for a good meal every once in a while for social purposes. If a person moves to a new place. They already have some preferences and taste. It would save both user and the food providers a lot of benefits if they live close to their preferred outlets. It is convenient for the owners and provide better sales and saves time for the user.
[2] Throughout the last few decades, researchers have examined the use of geo-location data to detect travel-related events and reasons. These research look at recurring GPS trajectories and use rules, models, and machine learning to identify personal movement patterns like home, work, shopping, and leisure. To get knowledge into the ongoing business processes, we are seeking to assess travel events as activities of various businesses in the current job.
[3] In recent years, there has been a noticeable surge in immigration. When these individuals arrive in the target nation, the majority of them are students who require long term lodging. However, because he is new to the area and does not know many relevant locations, this creates a difficulty. Therefore, this research article defines an effective methodology for Accommodation Recommendation through the use of K Nearest Neighbour Clustering along with Artificial Neural Networks and Decision Making. The experimental evaluation has been performed which has proved the superiority of the presented technique.




Methodology
In conducting an Exploratory Analysis of Geolocational Data, a comprehensive methodology can be structured around several key stages:
The initial step involves **Data Collection**, where datasets are fetched from relevant locations. This could encompass utilizing various sources like databases, CSV files, or APIs tailored to specific geographic data. Subsequently, the gathered data is subjected to the **Data Cleaning** process using Pandas, ensuring consistency, and eliminating inconsistencies or missing values that might impact subsequent analyses.
Once the data is prepared, the **Visualization** stage employs tools like Matplotlib, Seaborn, or Pandas to create informative boxplots, allowing for a clear understanding of the distribution and potential outliers within the datasets. Following this, integration with external data is pursued by fetching Geolocational Data from the Foursquare API, enabling a richer and more diverse dataset.
To unravel spatial patterns within the dataset, **K-Means Clustering** via ScikitLearn comes into play, facilitating the clustering of locations based on similarities, thereby uncovering potential groupings or clusters within the geospatial data.
Finally, to present the analyzed findings effectively, **Visualization on Maps** is employed. Tools such as Folium or Seaborn aid in the creation of visual representations on maps, providing a geographic context for the clusters identified through K-Means Clustering. This stage enhances the comprehensibility of the results, allowing for a clear depiction of the spatial distributions and clusters identified during the analysis.
This structured methodology ensures a systematic approach to explore, clean,  xanalyze, and visualize geolocational data, enabling the extraction of meaningful insights and patterns inherent in the dataset.

 
Fig 1
What is K-Means Algorithm?
K-Means Clustering is an Unsupervised Learning algorithm, which groups the
unlabeled dataset into different clusters. Here K defines the number of pre-defined
clusters that need to be created in the process, as if K=2, there will be two clusters,
and for K=3, there will be three clusters, and so on. It is an iterative algorithm that divides the unlabeled dataset into k different clusters in such a way that each dataset belongs only one group that has similar properties.
It allows us to cluster the data into different groups and a convenient way to discover the categories of groups in the unlabeled dataset on its own without the need for any training. It is a centroid-based algorithm, where each cluster is associated with a centroid. The main aim of this algorithm is to minimize the sum of distances between the data point and their corresponding clusters. The algorithm takes the unlabeled dataset as input, divides the dataset into k-number of clusters, and repeats the process until it does not find the best clusters. The value of k should be predetermined in this algorithm. The k-means clustering algorithm mainly performs two tasks: o Determines the best value for K centre points or centroids by an iterative process. o Assigns each data point to its closest k-centre. Those data points which are near to the particular k-centre, create a cluster. Hence each cluster has data points with some commonalities, and it is away from other clusters.




Proposed Methodology
Data Collection and Understanding:
Acquire the dataset provided, understanding the CSV values using the accompanying document. Assess the parameters from the codebook_food file, selecting the most relevant features that quantifiably differentiate students.
Data Cleaning and Feature Extraction:
Utilize Jupyter Notebook for data processing. Extract and preprocess the chosen relevant features into a Pandas data frame, addressing different value types and handling NaN values.
Data Visualization with Boxplot:\
Visualize the cleaned data frame using boxplots, interpreting trends observed in the population surveyed based on the codebook_food parameters. Analyze factors such as exercise habits, dietary preferences (vegetarian/non-vegetarian), and income to discern potential lifestyle patterns.
K-Means Clustering:
Implement K-Means clustering on the dataset, experimenting with various values of K to identify optimal clusters. Evaluate the clusters' demarcation based on attributes like income, observing differences as K values change. Record insights gleaned from boxplots.
Foursquare API Integration:
Create a Foursquare account and set up API credentials. Develop a query to identify residential locations within a specified radius around a chosen point (e.g., a sample location in Bangalore).
Visualization on Maps using Folium:
Apply the optimized K value to perform K-Means clustering on the prepared dataset. Utilize Folium to plot the clustering results on a world map, centering it on the selected location.
Design a distinct color scheme to differentiate cluster numbers effectively on the map visualization.
 
Fig 2
 Tab1

Fig 3




Result and Discussion
Prepared Pandas DataFrame for Analysis:
A cleaned Pandas DataFrame containing the relevant parameters extracted from the dataset ready for analysis in a Jupyter Notebook.
 
Tab 2
Boxplot Visualization and Insights:
A boxplot showcasing the cleaned dataset's distribution and trends.
Insights derived from the boxplot analysis, highlighting trends related to exercise habits, dietary preferences, income, or other significant parameters observed within the surveyed population.
 
Fig 4
Optimal K Value and Cluster Differentiation Parameters:
Identification of the optimal K value for K-Means clustering on the dataset.
Attributes or parameters based on which clusters are differentiated, highlighting key factors like income, lifestyle choices, or other distinguishing characteristics.
DataFrame with Location Data and Amenity Counts:
A DataFrame comprising latitude and longitude format locations.
Counts of amenities present around each location obtained through Foursquare API queries, providing insights into the surrounding facilities.
 
Tab 3
Map Visualization with Clustered Locations:
A map generated using Folium centered on the chosen location.Differentiation of locations by a distinct color scheme representing clusters obtained through K-Means clustering, resembling the reference screenshot for visual reference and analysis.
 
Bengaluru
 
Hyderabad



Conclusion
The exploration and analysis of geolocational data have unveiled a myriad of insights into demographic, lifestyle, and spatial patterns. Beginning with the acquisition and preprocessing of the dataset, meticulous cleaning and feature extraction were performed, focusing on parameters with substantial influence on identifying distinct characteristics among individuals.
Visualization, exemplified by boxplots, offered a clear depiction of distribution trends within the surveyed population, showcasing discernible patterns related to exercise habits, dietary preferences, and income levels. The application of K-Means clustering revealed distinct clusters within the dataset, highlighting significant attributes that delineate these clusters, such as income disparities or lifestyle choices.
Further integration with the Foursquare API provided a spatial dimension, enriching the dataset with information about surrounding amenities. The mapping of clustered locations using Folium illuminated geographical insights, visually representing clusters on a world map and enabling an understanding of their spatial distribution.
Overall, this project not only provided a comprehensive overview of the dataset but also unearthed valuable insights regarding the relationship between demographic attributes, spatial distribution, and lifestyle choices. These findings serve as a foundation for informed decision-making, allowing for targeted interventions or strategies tailored to specific demographic clusters within the studied population.
The amalgamation of data exploration, cleaning, analysis, and visualization techniques in this project underscores the significance of geolocational data in unraveling multifaceted insights and understanding complex human behaviors and preferences in various geographical contexts.
 
Fig 5
