# Function-approximation-with-the-help-of-genetic-programming
(GP) AI project

## Description:
One of the issues raised in mathematical sciences and engineering is function approximation. Approximation of the function means to approximate the mathematical rule of the said function by having the ability to calculate the value of an unknown function at arbitrary points. In this project, genetic programming (GP - Genetic Programming) is used to approximate the function.
## The goal of the project: to evaluate the level of mastery of the basic concepts of evolutionary algorithms (here, genetic programming)
One of the applications of GP is the approximation of functions. In this application, each member of the population represents a mathematical expression that is displayed in the form of a tree. The middle elements of this tree are mathematical, logical or any user-defined operators and the leaves of the tree contain constant values and input variables. The purpose of this application is to estimate the mathematical formula of an objective function. The objective function is a black box and the only thing we know (or can get) about it is to get the value of the function at arbitrary points. In this way, we find the value of the function at an arbitrary number of points and call them as a training set. For each tree, according to the values obtained for the training points and its difference with the real values, a merit value can be attributed and based on that, the evolutionary algorithm can be followed.
Operators used in trees should include at least the following (you can add more):
Bifunctional operators include: +, -, ×, /, ^ (power)
Single operation operators include: (x(cos), x(Sin
An example of a tree:
2.\pi +\left(\left(x+3\right)-\frac{y}{5+1}\right)

![image](https://user-images.githubusercontent.com/119484000/234824333-522c8dfe-9275-4217-8033-d20fca8d86bc.png)

## Program entry:
A number of training points and the output value of the objective function at those points (for simplicity, one-dimensional function in
is considered.)
## note 1 :
In practice, to generate input and evaluate the performance of the algorithm, one can consider arbitrary functions (including any operator that is predicted in the algorithm and even operators that are not predicted in the algorithm) and calculate the value of the function at an arbitrary number of points and these points considered as the input of the algorithm.
Be sure to test the case in which the input is generated from a function that has an operator that is not in the list of operators used in GP. For example, use the logarithm or tangent operator (or...) in the function rule used to generate test points, but these operators are not allowed in GP. Or remove the multiplication and division operator and in GP and generate the points with a function that has these operators.
## Note 2:
In one of the tests, generate test points by sampling an imaginary function in the form of a linear line (as in the figure below) and without having a specific rule for the function.

![image](https://user-images.githubusercontent.com/119484000/234824466-c4141cda-f5a1-4286-a5ef-bdd8ee858772.png)

## Note 3:
In one of the experiments, create a point or points of discontinuity in the function and check the difference in GP behavior. For example, you cannot use 2^x=y rule for points smaller than c1, and 3-x=-y rule for points between c1 and c2, and another function to generate training points for points larger than c2.
## Note 4:
In all cases, start with very simple examples and after making sure that the code is healthy, and the test method is healthy, move to more complex examples (!!) as much as possible.
## Note 5:
Your effort will have the main score and even if the results are not satisfactory, it is possible to get a full score if you spend time and learn the difficulties of the road. Also, if you get perfect results from all sections, it may cause a positive grade (extra grade).
## program output:
Display the formula corresponding to the best tree generated by the algorithm, the merit value of the best
Tree, number of generations, number of merit calculation, execution time.
