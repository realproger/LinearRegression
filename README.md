# Welcome to My Linear Regression


## Task
Getting and analysing existing data is the very first task of a data scientist.
The next step is to find tendencies and to generalize.

A linear model makes predictions by computing a weighted sum of the features (plus a constant term called the bias term):

y = hθ(x) = θT·x = θnxn + ... + θ2x2 + θ1x1 + θ0

• y is the predicted value. • n is the number of features. • xi is the ith feature value (with x0 always equals to 1). • θj is the jth model feature weight (including the bias term θ0). • · is the dot product. • hθ is called the hypothesis function indexed by θ.

### Closed-Form Solution

To find the value of θ that minimizes the cost function, we can differentiate the MSE with respect to θ. It directly gives us the correct θ in what we called the Normal Equation:

θ = (XT·X)-1·XT·y

(NB: This requires XTX to be inversible).

#### → Write a class LeastSquareRegression to calculate the θ feature weights and make predictions.

#### → Plot these points to get a feel of the distribution.

As you can see, these points are generated in a linear way with some Gaussian noise. Before calculating our weights, we will account for the bias term (x0 = 1).

#### → Write a function which adds one to each instance

## Gradient Descent

Reminder about Gradient Descent

As you may have noticed, our MSE cost function is a convex function. This means that to find the minimum, a strategy based on a gradient descent will always lead us to a global optimum. Remember that the gradient descent moves toward the direction of the steepest slope.

Writing a class to perform the gradient descent optimization

→ Plot the function f in 3D

→ Plot the progression of the gradient by using the history variable inside the class

We should clearly see the gradient moving toward the cavity of the function f !

→ How does the learning rate and the number of iterations influence the result ?

→ How to tune hyperparameters and choose a good learning rate?

→ What about the number of iterations? What is the Convergence Rate?

The batch gradient descent is good but suffers from a huge difficulty: it uses the whole training data set, which can be computationally and memory expensive. The time to train a model can be very long, Thus, a lot of variants of the implementation of the gradient descent exists to try to increase its efficiency. For example, a more light weight strategy is the Stochastic Gradient Descent.

### The Core Team



<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px'></span>
