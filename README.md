# PID-Control

1.	Describe the effects of components of PID class

In PID class, there are two functions called UpdateError and Totalerror. The first function updates values for the cte difference, cte and accumulated cte error.
CTE error is the main source to push the car toward the right direction. CTE difference is aimed to help car drive smoothly. And accumulated CTE error is to avoid system bias.

2. How hyper-parameter is chosen and some of my guess for further   improvement

In second function, we constructed a weighted average of the three errors as our optimization objective function. I found the coefficients by manually tuning with the help of the professor Sebastian’s lecture video. Though it works nice and seems easy to implement, I do believe we can try more sophisticated objective function alternatives since it’s essentially a multi-objective optimization problem. Another possible solution might be using machine-learning idea to train the model and find the most appealing coefficient with the help of enough training data.

