Example of a loss function is a mean squared error:

`C(w, b) >>> 1/2n * sum#x(|y(x) -a|^2)`

We focus on minimizing the function value rather than maximizing the correctness of the output (for example the number of correctly classified images), because with the loss function we know when we are scoring only marginaly better, even when the correctness of output stays the same.

This implies that we want to use a smooth function that we can derive.