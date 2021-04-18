Analytically finding the minimum of a function with many variables is very difficult. We are using algorithms like gradient descend to find it incrementally.

We are basically trying to reduce the [[Loss function]] `C` value at each step. That means that we want the `∆C = ∂C/∂v . ∆v` to be negative. The question is how to choose the `∆v` (`∆v` is defined as a transposed vector of all `v` changes - `(∆v#1, ∆v#2, ..., ∆v#n)^T`).

We define the gradient vector `∇C`  as a transposed vector of partial derivatives of all variables - `(∂C/∂v#1, ∂C/∂v#2, ..., ∂C/∂v#n)^T`. It relates changes in `v` to changes in `C`.

We then can define the change in loss function value `∆C ≈ ∇C . ∆v`. Then we define `∆v` in a way that helps us make `∆C` negative - `∆v = -η∇C`. I didn't get this on the first look, but `∆C ≈ ∇C . -η∇C` which equals  `∆C ≈ -η|∇C|^2` which is definitely negative for a positive `η` (learning rate).

Each move of the `v` then looks this: `v -> v' = v -η∇C` and if we keep doing this move over and over again the C will decrease or stay the same.

Some variations of gradient descend can more closely mimic the "ball-rolling-downhill" mechanism, but they are computationaly quite costly, because you need to compute second partial derivative and there is a squared number of variables of those derivatives.

We can now restate the gradient descent update rule in terms of weights and biases.

Because we would have to calculate the [[Loss function]] for all the training inputs when calculating gradient descend, we can use [[Stochastic gradient descend]] that estimates `∇C` by averaging from a randomly chosen sample of training inputs.

