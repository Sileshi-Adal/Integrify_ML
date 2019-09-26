<h1>From Eigenvalues to Optimization</h1>

1. What are the basic elements of optimization? Give some examples.
  
  <h6>A. Basic elements of optimization:
     1. Variables: Parameters which will be passed to optimization algorithm.
     2. Constraints: These are the boundaries within which the parameters (or some combination thereof) must fall
     3. Objective Function: This is the set of goal towards which the algorithm drives the 
     solution. For machine learning, often this amount to minimizing some error measure or maximizing
     some utility function.

    For example:

    Example question : The regular air fare between Boston and San Francisco is 500 dolars . An
    airline using
    planes with a capacity of 300 passengers on this route observes that they fly with an average of
    180 passengers. Market research tells the airlines’ managers that each $ 5 fare reduction would
    attract, on average, 3 more passengers for each flight. How should they set the fare to maximize
    their revenue? Explain your reasoning to receive credit.

    1. Variables : 1- Air fare which will be regulated 2- Quantity of passengers
    2. Constraints : Air fare should be regulated by preserving from making loss.
    3. Objective Function : Making the most profit arranging with number of quantity of passengers and   air fare
  
    B. Why is optimization important in machine learning? Give some examples. 
       Optimization is used to find more accurate results by using loss function. And in machine
       learning, Predicted values are deduced from some finite data. That's why optimization is very
       important for machine learning algorithms. **For example** while working on neural networks,
       arranging weight and type of nodes is done by result of optimization of
       loss function between predicted values and actual values. 
  </h6>

2. Recollect : What is a loss function /cost function? Give examples 

   Loss function or cost function is a function that maps an event or values of one or more
   variables onto a real number
   intuitively representing some "cost" associated with the event.Basically If predictions deviates
   too much from actual results, loss function would cough up a very large number. Gradually, with
   the help of some optimization function, loss function learns to reduce the error in prediction.
   **For example:** You have neural network which takes some data related to some house and predicts
   its price. Loss function is how predicted values deviates from the actual prices.


3. Essentially, the eigen operator is the differential operator. The eigenvalue represents the
   gradient of a cost-function's
   curve (i.e. from areas of high error descending to low error areas. The point of knowing this is
   to 1. determine which features are the best indicators for a range of outputs and 2. to know in
   which direction of eigenvalues to trend so that the cost function ultimately reaches its global
   minimum therby producing values with an error rate very very near 0.

4. The "Hessian" or "Hessian Matrix" is a list of values which represent the slope of the cost
   functions curve at a given
   data point. The Hessian values basically tell the algorithm 1. which direction comprises the
   steepest gradient toward a global minimum and 2. what direction that gradient is in.
   
5. The quadratic form elicits a parabola representing the error rate comparisons over a range for a
   cost/loss function which aids in understanding what optimization is trying to accomplish. Think
   of the Hessian value as being similarly related to an eigenvalue in that the eigenvalue is the
   radial distance from axis of points along an elipse. The Hessian value is the slope of a tangent
   line at a given point vs. the eigenvalue which is the radial distance from the central axis.
   Think of the maholonobis distance as being representative of the arc distance along the elipse
   from one point to another. To calculate the Maholonobis distance, one needs the radial distance
   or eigenvalue for both points. When computing the covariance, one inverts the precision matrix so
   as to compare covariance among different features in a data set. When computing the Hessian, the
   output values are representative of the slope of a tangent line at each eigenvalue along the
   elipse. This slope is representative of the shortest path to minimization/optimization. For the
   final question as to whther one could substitute the precision matrix for the Hessian, in short,
   no. The reason is as previously stated that we are no longer comparing the covariance of features
   to one another so much as we are comparing the cost function values to get an error rate which is
   very very near 0 or, contropositively a success rate very very near 1.
   
6. What is momentum and what problem is it solving? The Idea of Momentum in Machine learning is a
   method to increase the speed of training gradients, in other words it is a method, which helps
   to accelerate gradients vectors in the right directions, thus leading to faster converging. The
   main problems that momentum solves are handling of the noisy gradients and extremely small
   gradients in order to predict where the variable point will end up in time t.
