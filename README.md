# Analysis of FIRMS data for learning regression models

Our project focuses mainly on the collection of data, more specifically of temperatures and radiation, which will be analyzed by an intelligent agent that we have programmed and taught to predict forest fires. In addition to this, we will create a prototype application, which can be used by the inhabitants of Panama to report such forest fires. Informing the user about the numbers to call and what to do in case of a fire.

# How We Addressed This Challenge

For this challenge, we have implemented several prediction models and have been feeding them with data so that they can predict the occurrence of forest fires and a prototype application so that users can report the fires to the corresponding authorities.


We consider this important, as forest fires have a great impact on the economy and the environment. Because when these fires occur, economically there are many material losses, homes, jobs and, most importantly, lives and natural resources are lost.


Our model works by collecting temperature and radiation in pixels to predict the occurrence of the incident.

We use the pearson method to find some correlation in the data provided by the FIRMS database to find the best data to use in the training models (regression models).
To obtain the correlations between the data we have to:

1. The positive correlations: the data are related to each other. Yes,

one enhances the other as well.

2. Negative correlations: Data are inversely related, if

one fact increases the other decreases.

3. Correlations close to 0 : they are not related.



With this in mind we proceeded to the training by:


1. linear regression

2. ridge regression

3. K-neighbors regressor

4. random forest regressor: This was the model with the least prediction error and the highest score. Score: 0.88936536987672, Mean Absolute Error: 1.783584814892282

5. support vector regression


With this we hope to get the prediction data provided by NASA, help us to predict possible fires in Panama.


# How We Developed This Project

We were inspired to choose this challenge, because in addition to being interesting to use predictive models and a challenge, we consider the issue of wildfires important, especially after the last fires that occurred, which caused many losses and claimed many lives of wildlife in Australia and Brazil. We believe that it would be a good contribution to prevent fires of these magnitudes or at least to be able to discover them in time to control them.


To develop this project we used the Google Colab tool and the programming language used in the model was python. In the creation of the prototype of the APP we used JustmindPrototyper. Similarly keras program was used to debug the unnecessary information from the CSV files.


We had problems using the data, because it was not very clear, the temperature data are in the international system and at least in Panama they are used in centrigrades.


In the same way it was complicated for us to obtain the csv file. Since it took time to get to the mail for the download.


However, we obtained good results (not so bad) by training the data in different types of models.
# How We Used Space Agency Data in This Project

Data from the FIRMS of the country Panama was downloaded. In which we had some difficulty in understanding certain data, which were purified that would not be used in the project. We used external programs to improve the data.


The data helped us a lot, since there are no such exact files in other internet sites. 

# References
https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/active-fire-data

https://firms.modaps.eosdis.nasa.gov/tutorials/

https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/c6-mcd14dl#ed-firms-attributes

https://personal.us.es/vararey/adatos2/correlacion.pdf

https://idescubre.fundaciondescubre.es/noticias/disenan-programa-informatico-calcular-impacto-economico-los-incendios-forestales/

https://towardsdatascience.com/how-to-generate-prediction-intervals-with-scikit-learn-and-python-ab3899f992ed
