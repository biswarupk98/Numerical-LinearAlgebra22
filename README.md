# Numerical-LinearAlgebra22
# Problem 1:
In this problem you will test different algorithms for the least squares problem to approximate the function $f(t)=\sin (10 t)$ for $t \in[0,1]$ using a polynomial fit . To this end, first generate $m=100$ data points using the above function which forms your given data i.e $\left(t_i, f\left(t_i\right)\right.$ for $i=1 \cdots m$. Using this data, we would like to construct a 14 th degree least squares polynomial fit to $f(t)$. Determine its least square it using the following methods.
(a) Use QR Factorization with your implementation of Modified Gram Schmidt. You should write your own back substitution code for solving the resulting triangular system.
(b) Using QR Factorization with your implementation of Householder factorization.
(c) Using SVD (Computed with any inbuilt libraries in MATLAB/Python/Octave)
(d) Using normal equations, you can use backslash command in MATLAB to solve this system.

Accept the MATLAB/Octave/Python least squares solution (given by backslash "V" in MATLAB) as the truth. Display and plot the approximation given by this "true" solution and compare it with $f(t)$. Compare with the solution given by 4 methods described above. Explain the results.

# Problem 2:

A satellite revolving around one of the Saturn's moon Titan has unexpectedly found a new weird looking celestial body in its field of view, and the camera harbored in the satellite has taken a photograph of it and stored it as .jpg file. However, due to some technical difficulties it has not been able to transmit full resolution image in jpg format to earth. However, a simple onboard computer can be programmed from Earth remotely and the control station on Earth decided to use SVD to compress the image. This image is as below and also downloadable from Teams class page as a bmp file. As a scientist working to program the onboard computer, think about the following:
(a) How many singular values are required to approximate the image i.e., make it look indistinguishable from the original image? (Hint: Load the image in Python or Matlab or Octave or Julia and the matrix representation of the image will be accessible to you. For $r \times r$ pixel image, the image will have $r \times r \times 3$ matrix entries with the number 3 corresponding to color depth of the image representing Red, Blue, Green.)
(b) Based on your observation in (a), how many entries need to be transmitted to earth to reconstruct the approximate image as opposed to sending the original image?
[Perform the tasks in a programming environment comfortable to you like Matlab/Octave/Python/Julia. You can use inbuilt functions for computing SVD.]
(c) What is the 2-Norm and Frobenius-Norm error between the matrix representation of the original image and the approximate image obtained for different number of singular values. Check if the following theorems hold for these errors:

For the matrix $\mathbf{A}$ of rank $\mathrm{r}$, with singular values $\sigma_1, \sigma_2, \sigma_3, \ldots \sigma_r, \mathbf{A}_v$ is the $v$ rank approximation of $\mathbf{A} . \quad\left(\mathbf{A}_v=\sum_{i=1}^v \sigma_i \mathbf{u}_i \mathbf{v}_i\right)$ such that $1<v<r$, then: $\left\|\mathbf{A}-\mathbf{A}_v\right\|_2=\sigma_{v+1},\left\|\mathbf{A}-\mathbf{A}_v\right\|_F=\sqrt{\sigma_{v+1}^2+\sigma_{v+2}^2+\ldots+\sigma_\tau^2}$
