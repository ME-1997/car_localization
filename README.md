# Car detection and localization
Car detection and localization is used to detect bounding box where a vehicle exists, by using this data along with depth map -obtained by e.g,. LIDAR or stereo-vision- we can compute the nearest point hence determine distance toof collision.

The following approach is used:
1.	Extract HOG features from training data.
2.	Train SVM using cross-validation for parameters tuning.
3.	Use sliding window algorithm with different sizes.
4.  Obtain hot map from each window's vote
5.  Draw rectangle based on hot map

[Vehicles dataset](https://s3.amazonaws.com/udacity-sdc/Vehicle_Tracking/vehicles.zip)

[Non-vehicles dataset](https://s3.amazonaws.com/udacity-sdc/Vehicle_Tracking/vehicles.zip)

Sample Image:


![alt text](https://i.ibb.co/G70k5C9/Untitled3.png)



