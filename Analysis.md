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
