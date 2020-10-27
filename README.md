# VITMAV45_kishazi_3

Data is from the following URL: http://idojarasbudapest.hu/archivalt-idojaras

First, I tried to use the previous year's weather forecast, but after sawing the big difference between the years and in the oscillation, I just used the weather data from 2020.09.01 to 2020.10.20 which is called as '2020_tuning_data.csv'.

For the neural network I used the same solution that was shown on the lecture, just simplifying  a bit it, because I had less datapoints.

After I got a pretty accurate estimation I started to generate the future datapoints. Which was modifying the X_test array. Removing the first 20 part of 2D array from it and append a new one to the end of it. The new was the last on of the array appended with the predicted value for the last element of it. After these steps the following compliance is true about the future array:

2020.10.28 is gona be sample 58, at position 8 is 10.28
2020.11.03 is gona be sample 64, at position 14 is 11.03
2020.11.24 is gona be sample 85, at position 35 is 11.24

Which is show on the last plot combined with the past.
