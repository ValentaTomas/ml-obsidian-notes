Function predicting output based on input.

It takes **input** `X`, multiplies it by the **weight** `W`, sums it together with the **bias** `b` and returns it as the output `Y`.

![[neural-network.png]]

The mathematical representation is `Y = X * W + b`.

We can use the network for classification task by applying for example the [[Softmax]] .

When a neural network has more layers it is called a [[Deep learning]] network.

Neural network are used for state of the art [[Natual Language Processing]].

During training a [[Loss function]] is used for for evaluating the output.

[[Perceptron]] is a simple neural network cell with activation function that outputs 0 when the sum + bias of the cell is <= 0 and 1 when the sum + bias is > 0. The inputs of these cells must be 0 or 1.

[[Sigmoid neuron]] is a neuron which can have inputs between 0 and 1. The output of the neuron is calculated by [[Sigma Function]], outputing a number between 0 and 1, which can be used as an input for other sigmoid neuron.

[[Feedforward network]] is a network where the output from one layer is used as an input to the next layer. That means there are no loops in the network.

[[Recurrent Neural Network]] is a network where feedback loops are possible. Loops there don't cause problems, because the looped neuron output only affects inputs in a later time and for a limited duration. Learning algorithms for these networks are less powerful, but the networks are still useful.

We use the [[Gradient descend]] algorithm for finding the weights and biases so that the [[Loss function]] values is minimal.


