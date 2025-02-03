(Note: This was a group project created with Max, Sean and Jaden for our Machine Learning class)

Predicting Lap Times and Accidents for F1 World Championship Tracks

Formula 1 racing can be exciting to viewers and data scientists alike. For a competition where teams are invested in making improvements for a millisecond increase in performance, data can provide insights on how these improvements can be made. For our project we choose to focus on predicting accidents and lap times for the December 8, 2024 race in Abu Dhabi Grand Prix. 

As a long time fan, I’ve been following the races for a while and have noticed that some circuits are more susceptible to accidents than others. For instance, Red Bull Racing in Austria has the highest number of accidents accounting for its short circuit and sharp turns. Drivers average around 1 minute for a single lap while the average lap time for a F1 race is around 1.6 minutes. This tells us that circuit layout and design influence performance and safety. We also wanted to look into individual driver lap times and predict lap times for the December 8 race. 

For our predictive model, we trained our model from data available on Kaggle from 2013 to 2023. We split our data into training (2013-2023) and testing set (2024). Our key variables included:
	-circuits (circ_name, lap_limit)
	-driver specifics(driver_name, position_order)
	-race(year, month, avg_stop, diff_laps)
We utilized visualizations to show the relationship between average lap times and accidents happening across different circuits from 2013 to 2023. More technical circuits showed higher variability in lap times such as Monaco. We tried various models as a team and decided to go with a simple linear model to capture how circuit characteristics influenced pit stop efficiency and lap performance. We found some outliers that significantly skewed residuals so we excluded them to improve our model fit. We also added Oliver Bearman later to our training data since he was a new driver on the grid
participating for the first time in the 2024 season. Our model ended up with a R-square of 0.62 indicating our model predicts well without being overly complex. 
