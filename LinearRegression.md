###Linear Regression with one variable
m = number of training examples  
x = input features  
y = output variable / target variable  

(x, y) = refers to one training example  
x<sup>(i)</sup> y<sup>(i)</sup> refers to specific training example at index i. It doesn’t refer to an exponent.

h = hypothesis. function that maps x to y  
Predict that y is a linear function of x.  
<strong>y = h(x) = ϴ<sub>0</sub> + ϴ<sub>1</sub>x</strong>  

###Cost Function
J is the cost function  
ϴ<sub>i</sub> are parameters. the coefficients of the function.  
find values of ϴ<sub>0</sub> and ϴ<sub>1</sub> that minimize the cost (error) function.  
h(x) - y = difference in function versus actual… we want to minimize this.  
aka squared error cost function.  
J(ϴ<sub>0</sub>, ϴ<sub>1</sub>) = <<1/2m>> sum from i = 1 to m (h(x<sup>(i)</sup>) - y<sup>(i)</sup>)<sup>2</sup>  
find ϴ<sub>0</sub> and ϴ<sub>1</sub> that minimizes the error.  

Square the error because  
1) Squared gets rid of negative numbers that would cancel each other out.  Although you could use magnitude.  
2) For many applications small errors are not important, but big errors are very important.  example: self driving car. ½ foot steering error no big deal, 5 foot error fatal problem. So it’s not 10x more important… it is 100x more important.  


###Cost Function Intuition
simplify and make ϴ<sub>0</sub> = 0

###Gradient Descent
:=  (assignment operator, not equality)  
&alpha; = learning rate.  the learning rate controls the size of the adjustments made during the training process. 

