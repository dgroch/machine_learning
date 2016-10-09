# Assignment

1. Computing summary statistics of the data: Sketch summaries are techniques for computing summary statistics of data very quickly. In GraphLab Create, SFrames and SArrays include a method:

`.sketch_summary()`

which computes such summary statistics. Using the training data, compute the sketch summary of the ‘label’ column and interpret the results.

Q: What’s the least common category in the training data?
A: Birds

2. What is the nearest ‘cat’ labeled image in the training data to the cat image above (the first image in the test data)?

`reference_label = 16289`

3. What is the nearest ‘dog’ labeled image in the training data to the cat image above (the first image in the test data)?

`16976`

4. A simple example of nearest neighbours classification

For the first image in the test data (image_test[0:1]), which we used above, compute the mean distance between this image at its 5 nearest neighbors that were labeled ‘cat’ in the training data (similarly to what you did in the previous question).

sum
`180.778653548914`

mean
`36.15573070978294`


Similarly, for the first image in the test data (image_test[0:1]), which we used above, compute the mean distance between this image at its 5 nearest neighbors that were labeled ‘dog’ in the training data (similarly to what you did in the previous question).

sum
`188.85355680920784`

mean
`37.77071136184157`

**Accuracy of predicting dog in the test data: Using the work you did in this question, what is the accuracy of the 1-nearest neighbor classifier at classifying ‘dog’ images from the test set?**

67.8%
