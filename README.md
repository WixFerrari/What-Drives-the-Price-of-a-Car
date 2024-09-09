# What Drives the Price of a Car

The goal of this project is to determine the significant parameters influencing used car prices from a randomly sampled used car data base(426k). Multiple models will be created in order to find the factors that consumers value the most when purchasing a used car. The results found will be useful for car dealerships to optimize their inventory and pricing for the consumers, while maximizing profit and allowing them to understand what consumers are looking for.

# Summary:
The Ridge Regression seems to provide the best results with a mean R^2 of 0.167052, which narrowly beats out linear regression which was at 0.167026. The Lasso Regression performed very poorly and was the worst regression at 0.0202. Using five folds, Linear Regression R^2 scores: [ 0.25306752 0.28704258 0.32532795 -0.35870226 0.32839733] Ridge Regression R^2 scores: [ 0.25306835 0.2870537 0.32532607 -0.35858148 0.32839474] Lasso Regression R^2 scores: [ 0.02287283 0.03888373 0.02891428 -0.00693529 0.01744502] As it can be seen, Ridge has a slight edge over Linear regression while Lasso regression is performs very poorly.

Looking at the scatter plot of price vs odometer, histogram of car prices, and box plots from the data analysis,there are alot of outliers. Overall, the data was cleaned pretty well, but with more time I would have liked to revisit and potentially try and cut those outliers for more accurate results. I also would have liked to test out more categories vs price such as age of car vs price, as that would also give some additional info. Using other models such as random forests, decision tree, and etc in the future would also be very interesting and useful.

# Findings:
* The condition of a car matters. Cars that were like new and new typically had a higher price. When the condition gets worse, the price usually gets worse.
* The odometer matters as alot of cars sold were form the 10^4 to 10^5 miles range.
* Cars with lower odometer readings will have a higher price.
* Alot of the cars sold were priced from $20,000 and less.

# Next Step/Recommendations:
The next step would be to clean out those outliers and test brand vs price as well as age of car vs price. Most likely, brand and age of car will have a strong correlation to the pricing as people favor certain brands and prefer newer cars.

I had a lot of problems with the kernel dying, possible due to the size of the dataset, so any tips on how to prevent that in the future would be helpful.
