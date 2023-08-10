# Numerical-LinearAlgebra22
# Problem 1:
In this problem you will test different algorithms for the least squares problem to approximate the function $f(t)=\sin (10 t)$ for $t \in[0,1]$ using a polynomial fit . To this end, first generate $m=100$ data points using the above function which forms your given data i.e $\left(t_i, f\left(t_i\right)\right.$ for $i=1 \cdots m$. Using this data, we would like to construct a 14 th degree least squares polynomial fit to $f(t)$. Determine its least square it using the following methods.
(a) Use QR Factorization with your implementation of Modified Gram Schmidt. You should write your own back substitution code for solving the resulting triangular system.
(b) Using QR Factorization with your implementation of Householder factorization.
(c) Using SVD (Computed with any inbuilt libraries in MATLAB/Python/Octave)
(d) Using normal equations, you can use backslash command in MATLAB to solve this system.

Accept the MATLAB/Octave/Python least squares solution (given by backslash "V" in MATLAB) as the truth. Display and plot the approximation given by this "true" solution and compare it with $f(t)$. Compare with the solution given by 4 methods described above. Explain the results.
