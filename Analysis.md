# Classification Restricted Boltzmann Machines

The Classification Restricted Boltzmann Machine  models the joint distribution of an input x = (x1,..., xD) and target class y ∈ {1,...,C} using a hidden layer of binary stochastic units h = (h1,...,hH). This is done by first defining an energy function

<p align = 'center' height ='500px' weidth ='200'>
<img src ='https://github.com/Abhishekkakati101/Movie-Recommendation-System/blob/main/Assets/bltz1.PNG'>
</p>

with parameters Θ = (W,b, c,d,U) and where ey = (1i=y)
C
i=1
is the “one out of C” representation
of y. From the energy function, we assign probabilities to values of y, x and h as follows:

<p align = 'center'>
<img src ='https://github.com/Abhishekkakati101/Movie-Recommendation-System/blob/main/Assets/bltz2.PNG'>
</p>

where Z is a normalization constant (also called partition function) which ensures that Equation 1 is
a valid probability distribution. We will assume that the elements of x are binary, but extensions to
real-valued units on bounded or unbounded intervals are straightforward.
Unfortunately, computing p(y,x,h) or p(y,x) is typically intractable. However, it is possible to
sample from the ClassRBM, using Gibbs sampling, that is, alternating between sampling a value
for the hidden layer given the current value of the visible layer  (made of variables x and the ey
representation of y), and vice versa. All the required conditional distributions are very simple.
When conditioning on the visible layer, we have

<p align = 'center'>
<img src ='https://github.com/Abhishekkakati101/Movie-Recommendation-System/blob/main/Assets/bltz3.PNG'>
</p>
