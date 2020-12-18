# ada-2020-project-milestone-p3-p3_runtime-error
ada-2020-project-milestone-p3-p3_runtime-error created by GitHub Classroom

## Title: where do the globetrotters come from?
 
### Abstract:

<p align="justify">The exponential increase of global interactions among people, caused by globalisation, lead to a dramatic change in our daily life, transforming our social, political and economic structure. 
Our travelling habits are no exception in the radical changes we underwent in past few decades, the rapidity and facility with which we can reach nearly every part of the world has encouraged people to travel more, further and differently than in the past. 
Being able to identify the predominant human fluxes and new travelling habits of citizens could be highly beneficial in a plethora of sectors and domains. For instance, never as today we can understand the importance of modelling the spreading of a virus across the world, only achievable with a solid knowledge of the peoples’ movements within and among countries. With these pieces of information governments could put in place ad hoc containment measures potentially more effective, as based on the true behaviour of human beings. In a business context, deeper knowledge of human mobility could be insightful to investigate the most and least popular travelling routes, in order to efficiently allocate resources and establish prices for example. For social studies, the study of the incoming and outgoing fluxes could reveal precious information on a population’s culture and habits.</p>
There are clearly multiple approaches to investigate human mobility across the world, the one we are going to follow is based on the data gathered by two social networks, namely Gowalla and Brightkite, for which we have available a set of users and respective check-ins locations. 
By relating the latitude and longitude coordinates of check-ins to the respective countries where the localization took place we can investigate the users’ movement, potentially in the home country and abroad. </p>
 
### Research questions: 
1. What are the main fluxes of people over the world ?
2. Have some countries different trips habits than others ?
3. What is the influence of factors like the language, the distance or the GDP on travlling habits ?

### Datasets used 

[Check-ins from Gowalla](https://snap.stanford.edu/data/loc-gowalla.html) 

[Check-ins from Brightkite](http://snap.stanford.edu/data/loc-brightkite.html)

[Country Mapping - ISO, Continent, Region](https://www.kaggle.com/andradaolteanu/country-mapping-iso-continent-region)

[Countries of the world](https://www.kaggle.com/fernandol/countries-of-the-world)

[Language list by country and place](https://www.kaggle.com/zinovadr/language-list-by-country-and-place?select=Language+List+by+Country+and+Place.xlsx)

[Continent - Country](https://www.kaggle.com/sarques/conticountry)
 
### Method:
1. Get the previous results that we had about home locations of users
2. Each check-in and each home location is associated to a country (and therefore a continent) thanks to the **reversed_geocoder library** (which takes coordinates as input as country code as output)
3. Define the **geographical boundaries** (list of countries) : the study is relevant only in countries where we have enough data. We will therefore focus our study on countries where at least 1 citizen over 100 000 is on the social networks (Gowalla and Brightkite). This give us a list of 25 countries. 
4. Compute the number of travelers coming from this list of 25 countries and going anywhere in the world. The resulting dataframe contains the features "home_country", "foreign_country", "number_of_users". 
5. Understanding what drives people when they travel. To achieve this, we collected data about distances between countries : what is the **distance** between them, do they speak the same **language**, what is the **difference of GDP**. 
6. **Polynomial regression** in order to draw conclusions about the three previous factors.
7. With the collected data, some **traveling statistics** and **fluxes maps** are presented. Especially a **comparison between Europe and the United-States** and an **analysis of mobility fluxes** of the countries for which we had the more data. 

### Timeline :

-    Week 1 :
1. Distribution of homes in the world  
2. Definition of the geographical boundaries of our study

-    Week 2 :
1. Computing the main dataframe : number of travelers between pairs of countries
2. Computing the 3 parameters : distance, languages and GDP.
3. Polynomial regression. 

-    Week 3 : 
1. Maps of fluxes 
2. Write our data story
3. Write a clear notebook 
4. Begin the communication video 

### Organization within the team : who did what ?

Chiara :
- Definition of the geographical boundaries of our study
- Polynomial regression
- Maps of fluxes 
- Write our data story
- Write a clear notebook
- Work on the communication video

Cyril :
- Distribution of homes in the world
- Computing the main dataframe : number of travelers between pairs of countries
- Maps of fluxes
- Write our data story
- Write a clear notebook
- Work on the communication video

Matthieu :
- Computing the main dataframe : number of travelers between pairs of countries
- Computing the 3 parameters : distance, languages and GDP.
- Polynomial regression
- Write our data story
- Write a clear notebook
- Work on the communication video
