# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> This is a regression problem, the outcome is a quantitative variable. We'd be interested in inference as we want to understand the relationship between predictors & response, not predicting. The number of observations is 200, the amount of reserves, and we have 4 predictors (size, years, budgest, proximity).

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> The is a classification problem, the outcome is a qualitative variable, successful or not. We'd be interested in prediction so we can know if the proposed corridor will be successful. We have 30 observations and 11 predictors (width, length, land use type, 8+ others).

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> This is a regression problem, ozone concentration is a quantitative variable and we want to predict future ozone concentration. As we have collected weekly average data, we have 52 observations for 2019. There are four predictors, SST, wind, solar radiation, and atmospheric [pressure?].

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> Flexible regression methods captures non-linear relationships and potentially more complex relationships. This can lower bias as we could fit the true underlying function more closely and potentially make better predictions. However, these methods are sensitive to noise, can result in overfitting, and require more data to reliably compute. Thus, these are preferred when a lot of data is available, the true relationship is non-linear, and prediction is the goal. The lesser flexible methods are preferred when data is limited, you have knowledge the relationship is linear, and inference is the goal.

---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> Parametric approaches assume a function exists for the true form of the underlying function, while non-parametric approaches don't make this assumption. For example, linear regression assumes the underlying function is linear. Some advantages for parametric methods are simpler and easier to interpret, with parameter coefficients, standard errors, and p-values. The disadvantage come in when models are misspecified or completely wrong. For example, if the underlying function is not linear but assumed so, estimates will be biased and misleading, a linear model is unable to capture any non-linear relationship.