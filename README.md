# Fly Higher

![flights1](https://user-images.githubusercontent.com/39362431/126262393-8d631f0b-616a-4ead-86d1-865e84b5e7c0.JPG)


![flights2](https://user-images.githubusercontent.com/39362431/126262477-060326fa-6503-4f1d-bcf1-c1cb28da9068.JPG)


Air travel has always in the need of constant prejudice against the several factors that go into framing the prices. Here, we take historical flying data from a resource (find dataset reference below), and predict the corresponding prices of flights using the historical information. We test our data upon several models to check for the highest amount of accuracy and good recall values.
- We train our model using the several parameters present in the dataset to adapt to changes in prices subject to flight source, destination, journey timings, time of the day, number of layovers, amongst several other factors.
- We clean the incoming data and split and train it using several entities discovered during Exploraratory Data Analysis. Over time, we build a model with some optimised parameters and hyperparameters to arrive at a solution.
- After verifying the model on the test set, we are ready to publish the model. We generate an h5 model.save() file and export it into our current file system. This helps us to test the model at our own discretion, from any system, online or offline.
- Having had experience in building only front end systems, I struggled into this part. I had to learn a bit of Flask, just enough over the course of a few days to actually allow me to create a web-page out of the h5 model I created. Having the visual model present in the browser was a treat for me indeed.
- Finally, I decided to go on and deploy the app. Here was where my limited knowledge show through. I had tried to follow the general route of deploying Flask Files on the web through Heroku, but that's where I faced the problem. I learnt about the Heroku library, and how to deploy Flask and Django apps as easily as a command line script. Just like creating the Flask web app in the first place. But the major problem was, in Heroku, I had to link my GitHub Repository to the Heroku project, and apparently I couldn't get to upload the H5 model file on Github. This was due to GitHub's policy of not being able to upload a single file above 25 MB of size.
- Solving the problem: I am in the process of exploring the Google Cloud Platform as well as the Azure Cloud to deploy my ML based web apps, as these environments allow me cloud storage, enough to actually store my 50 MB h5 model in them already. Apart from that, following the Heroku route is still possible. There's a second option of using GitHub LFS(Large File Storage) that seems to solve the problem, by allowing to upload bigger files. But for some reason, I can't get a version that runs properly on my Pop OS 19.10 system. I'm working on solving the problem through either route now, but more inclined to the Google Cloud Platform, as I understand the plethora of advantages it has over GitHub LFS standard approach.
- Lastly, I understand that the owing to the current pandemic and closely studying the influence on air ticket prices, it's only positive to say that ticket prices have taken a major hit. As our dataset is based out of historical data, and due to absence of such a historic event previously, flight prices might be a bit off from our model. But they do give us the general idea. I am studying about how the flight prices increased during the COVID-19, and by how much on a bounce of probabilities.


Dataset Link - https://www.kaggle.com/nikhilmittal/flight-fare-prediction-mh/

*Thank you!*

*Somdev Basu*

