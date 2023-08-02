# daml_nb
### Data Analysis + Machine Learning Jupyter Notebooks
Repository for list of data analysis and machine learning jupyter notebooks from courses that I attended (or am attending), and additional work done for the dataset beyond what was required. 

This will also include datasets I found interesting from other sites. 

### supermarket.ipynb
This `.ipynb` (and `.ppt` not included here) was done in fulfillment of BCG RISE 2.0 Part-time Business & Data Analytics Capstone Project. Client data has been anonymized fully for the data visualization. 

Thus, results from this set of analysis might not make sense. But the concepts of analysis and story-telling used here were done similarly to what we did for the client. There are some variations on the presentation style and data presented to account for the fact that the project was a team effort but this presentation with the NTUC FairPrice data was an individual one.

### sms.ipynb
This `.ipynb` is a personal project to explore NLP N-gram and word embedding using the SMS Corpus available on Kaggle. Dataset link is included in the notebook. There is an accompanying `.ppt` available upon request.

### bike_sharing/
This is an exploratory data analysis project using ridership data from Divvy, a bike sharing system, in Chicago, US. The data can be obtained from the [link](https://divvy-tripdata.s3.amazonaws.com/index.html) here. The data from Divvy contains the trip details, like the bike stations and trip durations etc. Additional [geocode](https://console.cloud.google.com/apis/library/geocoding-backend.googleapis.com) and [weather](https://console.cloud.google.com/marketplace/product/noaa-public/gsod) data from the Google Cloud Platform are included in. GCP was chosen as other geocoding and weather APIs on the net are subscription-based while GCP offers a 3-months free trial. 

The analysis is splitted into two notebooks, one for retrieving data and preprocessing, another for the exploratory descriptive analysis of the data.

The main hurdle for this analysis is the retrieval of accurate geocodes based on the bike station names. As the bike station names and the actual locations at which the stations are located are different, and GCP geocoding API returns slightly different outputs on runs from different days, the geocodes in this analysis are not 100% accurate. It would be best if Divvy has an additional station dataset that comes with the latitude and longitude data of the bike stations.

The main objective of this analysis mainly lies with retrieving data from different sources (Divvy and Google Cloud) and combining the data for meaningful descriptive analysis of the whole dataset. Main questions would be how riders' behaviours change over different seasons, which are the most popular stations and trips and the demographics, trip duration and distance distributions of the riders. 