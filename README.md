# Is There Parking?

This model attempts to answer whether there is parking or not on an average residential street using 
images taken of a street over the last 8 weeks. The images were taken at different times of day and day 
of the week, but from the same angle.

First, we compressed the images using k-means clustering. Each image was compressed, or reduced, to $k = 2,3,4,8,16,32$ colors. Next, we chose all the images compressed by $k$ clusters and run ISOMAP and PCA 
dimensionality reduction techniques on the set of image arrays. Lastly, we used a Gaussian Mixture Model (GMM) to classify the images as having available parking or unavailable parking.
