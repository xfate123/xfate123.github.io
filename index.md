#My First Post

##About the calibration property of logistc regression

When I study classification machine learning models, I always ask myself how we define a good classifier?
Good accuracy rate? Not true, especially for unbalanced data
Precision and Recall?Not true, cause we manipulate this metrics by changing the threshold.
ROC_AUC? Yes,cause this metric is independent of threshold, only mesure the ability of the model to rank data point from one class over datapoint from another class.
Is that it? No!
I always think RF or gradient boosting are better classifier compare to logistic regression, cause those ensemble classifers usually have higher ROC_AUC, also can handle extreme unbalanced data. Bur logistic regression has a super skill, well-calibration.
So what is well calibrated mean?
Using corona virus as the example. Imagine I invent a toolkit to test the corona virus. Even though this toolkit can not 100% percent accurate to test the cornoa virus, but if it is well-calibrated, it can precisively estimate the infected rate and total infected people.
Why does logistic regression can have such special skill?
Let's look at the equation of logistic regression.
log(odds)=a+b1*x1+b2*x2+b3*x3.......+bn*xn
This is a linear regression, then we can assume odds is unbiased.
Accoding to central-limit theorem, the sample mean of odds follow a normal distribution of which mean is popuplation odds.
Well-Calibrated is a very important property for some sepcial case.
Then can we make the models don't have this feature become well-calibrated? Yes, we can
I will post another airticle to about this in detail.
To be continued
