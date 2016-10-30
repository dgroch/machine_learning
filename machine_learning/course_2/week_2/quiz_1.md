# Quiz 1

*Q1: Which of the following is NOT a linear regression model. Hint: remember that a linear regression model is always linear in the parameters, but may use non-linear features.*

y=w0w1+log(w1)x

*Q2: Your estimated model for predicting house prices has a large positive weight on 'square feet living'. This implies that if we remove the feature 'square feet living' and refit the model, the new predictive performance will be worse than before.*

False

*Q3: Complete the following: Your estimated model for predicting house prices has a positive weight on 'square feet living'. You then add 'lot size' to the model and re-estimate the feature weights. The new weight on 'square feet living' [_________] be positive.*

Might

*Q4: If you double the value of a given feature (i.e. a specific column of the feature matrix), what happens to the least-squares estimated coefficients for every other feature? (assume you have no other feature that depends on the doubled feature i.e. no interaction terms).*

They stay the same

*Q5: Gradient descent/ascent is...*

An algorithm for minimizing/maximizing a function

*Q6: Gradient descent/ascent allows us to...*

Estimate model parameters from data

*Q7: Which of the following statements about step-size in gradient descent is/are TRUE (select all that apply)*

If the step-size is too large gradient descent may not converge AND If the step size is too small (but not zero) gradient descent may take a very long time to converge

*Q8: Let's analyze how many computations are required to fit a multiple linear regression model using the closed-form solution based on a data set with 50 observations and 10 features. In the videos, we said that computing the inverse of the 10x10 matrix HTH was on the order of D3 operations. Let's focus on forming this matrix prior to inversion. How many multiplications are required to form the matrix HTH?*

features by features
10 x 10 = 100 (incorrect)

observations by features
50 x 10 = 500 (incorrect)

(observations x features) x (features x observations)
(50 x 10) x (10 x 50) = 250,000 (incorrect)

*Q9: More generally, if you have D features and N observations what is the total complexity of computing (HTH)−1?*

O(D^3) (incorrect)
O(N x D^3) (incorrect)
O(N^2 x D) (incorrect)