# machine-learning-exercise-5-solved
**TO GET THIS SOLUTION VISIT:** [Machine Learning Exercise 5 Solved](https://www.ankitcodinghub.com/product/machine-learning-labs-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;110195&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Machine Learning  Exercise 5 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Machine Learning Course

Goals. The goal of this exercise is to

• Do classification using linear regression.

EPFL

www.epfl.ch/labs/mlo/machine-learning-cs-433

• Implement and debug logistic regression using gradient descent.

• Compare it to linear regression.

• Implement Newton’s method for logistic regression.

Setup, data and sample code. Obtain the folder labs/ex05 of the course github repository

github.com/epfml/ML course

We will use the dataset height weight genders.csv in this exercise, and we have provided sample code templates that already contain useful snippets of code required for this exercise.

• The logistic function (a.k.a. sigmoid): σ(x) := (1 + e−x)−1

• The derivative of the logistic function is:

• The logistic regression predicts y ∈ {0,1} with the following probability

p(y = 1|w,x) = σ(x⊤w) p(y = 0|w,x) = 1 − σ(x⊤w).

• The negative log-likelihood loss for the binary classification problem (a.k.a. cross entropy loss) is:

where yi ∈ {0,1} for all i.

1 Classification Using Linear Regression

We will try to use linear regression to do classification. Although this is not a good idea in general (as discussed in the class), it will work for simple data. Concretely, we will use the height-weight data from the first exercise to predict the binary valued gender (sex). For better visualization, we will randomly sample 200 data points from the data.

Exercise 1:

Classification using linear regression.

• Use least squares(y, tx) from the previous exercise to compute the weights w on the height-weight data. Please COPY your previous implementation to the template file of this exercise least squares.py.

• Visualize the data points and the decision boundary with visualization() as in Figure 1.

Figure 1: classification by least square.

2 Logistic Regression

Exercise 2:

Implement logistic regression using gradient descent.

• Fill in the notebook function sigmoid().

• Fill in the two notebook functions calculate loss() and calculate gradient(). The first function should return the negative log-likelihood loss, while the second function should return the gradient of this loss w.r.t. the parameters w.

• Implement gradient descent learning by gradient descent() for logistic regression. You should calculate the loss and its gradient w.r.t. w. Now, you can update the weights w, and the function should return the loss and these updated weights w.

• Plot the predictions to get a visualization similar to the right part of Figure 1. Check if you get similar or different results.

Now that we have gradient descent, we can easily implement Newton’s method.

Exercise 3:

Newton’s method for logistic regression

wt+1 = wt − γ∇2L(wt)−1∇L(wt).

• Fill in the notebook function calculate hessian(). Now, complete logistic regression() by using calculate loss(), calculate gradient() and calculate hessian(). This function logistic regression() should return the loss, gradient, and Hessian. Note that it should not update nor return the parameters w. • Your gradient descent code can now be turned into a Newton’s method algorithm to find the optimal parameters w. Please fill in the notebook function learning by newton method(), which does a single parameter update. The function should return the loss and the updated parameters. hint: Use np.linalg.solve instead of directly computing the inverse ∇2L(wt)−1.

2

Exercise 4:

Penalized logistic regression.

• Fill in the notebook function penalized logistic regression(). This requires you to add the regularization term λ∥w∥2. As a sanity check, set λ to a very small value and see if it gives the same result as before. Once complete, please fill in the notebook function learning by penalized gradient(), and increase the value of λ and check whether (the norm of) w is shrinking or not.

• Check if this gives the same answer as gradient descent. To debug, print the function value and the norm of the gradient in every iteration. All these values should decrease in every iteration.

3
