# ada-2020-project-milestone-p3-p3_runtime-error
ada-2020-project-milestone-p3-p3_runtime-error created by GitHub Classroom

## Title: where do the globetrotters come from?
 
### Abstract:

Being able to identify the predominant human fluxes and mobility patterns in the world is crucial for effectively modelling the spreading of diseases, establishing effective mobility connections and understanding the travelling habits of different populations. This project extension continues the exploration of human geographic movement by relating the latitude and longitude coordinates of check-ins (to the Gowalla and Brightkite social networks) to the respective countries where the localization took place. This is done with the purpose of investigating human migration patterns within and among countries. We are looking for eventual correlation between the users’ home location and their travelling destinations, possibly identifying what are the most frequent connections among countries.  
 
### Research questions: 
Can we detect particular mobility patterns (fluxes) among countries?
-   	Do people tend to mostly travel within their country, do they go abroad? how often? and to where? 
-   	What is the percentage of users traveling to a specific country?Are there privileged travelling destinations ?

### Proposed Dataset:
The dataset which will be used in order to carry out the investigation are: 
Gawalla check-ins: users’ check-ins to the Gawalla social network (Friendship and mobility article) 
Brightkite check-ins : users’ check-ins to the Brightkite social network (Friendship and mobility article) 
Country dataset: country name, population, area and literacy from tutorial 1 (happiness) (I have not found a link)
 
### Method:
As a first step, it will be necessary to associate to each latitude and longitude coordinates of check-ins the specific geographical location (continent, country, city..). This could be carried out by the use of the GeoPy library. 

Secondly, it will be necessary to carry out a preliminary  study on the distribution of the users’ houses in the world (users’ houses already identified in P2) in order to understand which are the most represented countries, and whether the analysis should be focused only on a narrower set of countries. Specifically, this could be done by identifying which percentage of the country’s population is represented by the check-in dataset and potentially discard the poorly represented regions (country_info dataset for population). 
 
For each user it will be necessary to create a list of visited countries, excluding the one of the home location. 

Proceed by analysing the data trying to answer the specific research questions. 

### Timeline :

-    Week 1 :
distribution of homes (=> definition of the boundaries of our study)
calculation of the ratio of people who did not travel

-    Week 2 :
list of destinations for each user
migration data calculation 

-    Week 3 : 
Report/data story
notebook 
video 

### Organization within the team :

-    Week 1 :
Distribution of homes (1 pax)
Ratio of people who didn’t travel (1 pax)
Visualization (1 pax)

-    Week 2 :
Destinations and migration data computation (1 pax)
Visualization and interpretation (2 pax)
