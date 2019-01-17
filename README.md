
# KNN with Scikit-learn

## Introduction

In this lesson, we'll explore how we can use sklearn's implementation of K-Nearest Neighbors for both Classification and Regression, as well as some best practices for using the algorithm. 

## Objectives

You will be able to:

* Use KNN to make classification predictions on a real-world dataset
* Perform a parameter search for 'k' to optimize model performance
* Evaluate model performance and interpret results

## Why Use sklearn?

Since KNN is a simple algorithm, and one that we've already written our own implementation of, you may be wondering why we should even bother using sklearn when we have already written our version of KNN. The answer lies in optimization. We implemented a very bare-bones, scrappy version of KNN. However, there is much room for improvement! Sklearn, on the other hand, is maintained by a team of the best data scientists, researchers, and machine learning engineers in the world! Building your own implementation of any machine learning algorithm is valuable experience, and can provide great insight into how that algorithm works, and how we can best use it.  However, in general, you should always use professional toolsets such as sklearn whenever possible--their implementations will always be best-in-class, in a way a single developer or data scientist simply can't hope to rival on their own. In the case of KNN, you'll find sklearn's implementation to be much more robust and fast, because of optimzations such as caching distances in clever ways that their algorithm performs under the hood. 

## Using the sklearn Docs

As a rule of thumb, you should familiarize yourself with any documentation available for any libraries or frameworks you use. Sklearn provides some of best documentation in the world. For every algorithm, you'll find a general [documentation page](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html) which tells you things such as the inputs, parameters, outputs, and caveats of any algorithm. However, you'll also find very informative [User Guides](https://scikit-learn.org/stable/modules/neighbors.html#classification) that explain both how the algorithm works, and how to best use it, complete with sample code! 

For example, the following image can be found in the sklearn User Guide for K-Nearest Neighbors, along with an explanation of how different parameters can affect the overall performance of the model. 

<img src='knn_docs.png'>

## Best Practices

Although we did just about everything from scratch in section, you'll find that sklearn provides robust implementations for things such as evaluation metrics.  No need to worry about calculating your own F1-score--there's a function for that! 

In general, in the next lab, you'll want to focus on the overall Data Science Process--not get bogged down in the implementation of any one algorithm. In the final lab for this section, we'll focus on loading, exploring, cleaning, modeling, and evaluating a dataset from start to finish. Try to focus on the following questions:

* What decisions do I need to make regarding my data? How might these decisions affect overall performance?

* Which predictors do I need? How can I confirm that I have the right predictors?

* What parameter values (if any) should I choose for my model? How can I find the optimal value for a given parameter?

* What metrics will I use to evaluate the performance of my model? Why?

* How do I know if there's room left for improvement with my model? Are the potential performance gains worth the time needed to reach them?


## A Final Note

After cleaning, preprocessing, and modeling the data in the next lab, you'll be given the opportunity to iterate on your model. Although this section is optional, we **_highly recommend_** you give it a try! Building a model is the easy part--figuring out how to improve it is where the the real challenge lies. 

## Summary 
If you're not sure where to start, as an example, ask yourself some basic questions such as "will my results be different with unscaled data?", and then fit another model to unscaled data to answer it! Eventually, you'll start to recognize patterns that will help you gain a more complete understanding of the algorithms you're using, as well as a more complete understanding of data science as a process!
