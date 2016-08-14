###Chapter 1. Giving Computers the Ability to Learn from Data
第一章，给于计算机学习数据的能力

In my opinion, machine learning, the application and science of algorithms that makes sense of data, is the most exciting field of all the computer sciences! We are living in an age where data comes in abundance; using the self-learning algorithms from the field of machine learning, we can turn this data into knowledge. Thanks to the many powerful open source libraries that have been developed in recent years, there has probably never been a better time to break into the machine learning field and learn how to utilize powerful algorithms to spot patterns in data and make predictions about future events.


在我看来，机器学习(应用和算法科学是数据有意思)是所有计算机科学中最令人激动的领域。
我们生活在数据大量冗余的年代，使用机器学习中的自学习算法我们可以将数据转换为知识。
感谢众多近几年被开发的强大的开源库，使进入机器学习领域和学习如何使用强大算法来为数据分离以及预测未来事件，成为可能。


In this chapter, we will learn about the main concepts and different types of machine learning. Together with a basic introduction to the relevant terminology, we will lay the groundwork for successfully using machine learning techniques for practical problem solving.


在本章中，我们将学习机器学习的主要概念和分类。同时简单介绍下相关术语，我们将依靠基本原理来成功使用机器学习技术解决实际问题。


In this chapter, we will cover the following topics:
本章有以下几个主题
```
####The general concepts of machine learning 机器学习的一般概念
####The three types of learning and basic terminology 三种学习类型和基本术语
####The building blocks for successfully designing machine learning systems 成功设计机器学习系统的积木
####Installing and setting up Python for data analysis and machine learning 安装和搭建Python环境为数据分析和机器学习
```

Building intelligent machines to transform data into knowledge
搭建智能机器将数据转变为知识


In this age of modern technology, there is one resource that we have in abundance: a large amount of structured and unstructured data. In the second half of the twentieth century, machine learning evolved as a subfield of artificial intelligence that involved the development of self-learning algorithms to gain knowledge from that data in order to make predictions. Instead of requiring humans to manually derive rules and build models from analyzing large amounts of data, machine learning offers a more efficient alternative for capturing the knowledge in data to gradually improve the performance of predictive models, and make data-driven decisions. Not only is machine learning becoming increasingly important in computer science research but it also plays an ever greater role in our everyday life. Thanks to machine learning, we enjoy robust e-mail spam filters, convenient text and voice recognition software, reliable Web search engines, challenging chess players, and, hopefully soon, safe and efficient self-driving cars.

现代技术，只有一种资源我们拥有的是冗余的：大量结构化和非结构化数据。在20世纪后半世纪，机器学习变革成人工智能的一个子领域：包括开发自学习算法以从数据中获得知识为预测。相比人手工准守职责和从分析大量数据建模，机器学习提供了一种更有效的可选的手段在数据中来捕捉知识以优雅地改善预测模型的性能，使决策数据驱动化。不仅机器学习在计算机科学研究中变的越来越重要，在我们日常生活中它也扮演了更伟大的角色。 感谢机器学习，让我们享受鲁棒的垃圾邮件过滤器，方便的文本和声音识别软件，可信的Web搜索引擎，挑战围棋手，以及希望不就将来可以实现安全高效的自动驾驶汽车。


The three different types of machine learning
三种不同类型的机器学习（ 非监督学习、监督学习、强化学习 ）
In this section, we will take a look at the three types of machine learning: supervised learning, unsupervised learning, and reinforcement learning. We will learn about the fundamental differences between the three different learning types and, using conceptual examples, we will develop an intuition for the practical problem domains where these can be applied:
在这一节中，我们将看下三种类型机器学习：监督学习、非监督学习、强化学习。
我们将学习三种学习类型的不同，并且使用例子我们将解决一个直觉感觉它们可以应用的实际问题



Making predictions about the future with supervised learning
使用监督学习来做预测
The main goal in supervised learning is to learn a model from labeled training data that allows us to make predictions about unseen or future data. Here, the term supervised refers to a set of samples where the desired output signals (labels) are already known.
监督学习的主要目标是从打标签的训练数据中学习一个模型，以使我们对未看到/未来数据做预测。这里，术语监督指的是一个含有期待输出信号/标签已知的样本集

Considering the example of e-mail spam filtering, we can train a model using a supervised machine learning algorithm on a corpus of labeled e-mail, e-mail that are correctly marked as spam or not-spam, to predict whether a new e-mail belongs to either of the two categories. A supervised learning task with discrete class labels, such as in the previous e-mail spam-filtering example, is also called a classification task. Another subcategory of supervised learning is regression, where the outcome signal is a continuous value:
考虑到垃圾邮件过滤的例子，我们可以使用监督学习算法在一系列被正确标记邮件上训练一个模型，以预测一封新邮件属于垃圾邮件还是正常邮件。一个针对有离散类标签的监督学习任务，比如在之前垃圾邮件过滤的例子中，也被叫做一个分类任务。另外一个监督学习的子类是回归，回归中的输出是一个连续值



Classification for predicting class labels
Classification is a subcategory of supervised learning where the goal is to predict the categorical class labels of new instances based on past observations. Those class labels are discrete, unordered values that can be understood as the group memberships of the instances. The previously mentioned example of e-mail-spam detection represents a typical example of a binary classification task, where the machine learning algorithm learns a set of rules in order to distinguish between two possible classes: spam and non-spam e-mail.

However, the set of class labels does not have to be of a binary nature. The predictive model learned by a supervised learning algorithm can assign any class label that was presented in the training dataset to a new, unlabeled instance. A typical example of a multi-class classification task is handwritten character recognition. Here, we could collect a training dataset that consists of multiple handwritten examples of each letter in the alphabet. Now, if a user provides a new handwritten character via an input device, our predictive model will be able to predict the correct letter in the alphabet with certain accuracy. However, our machine learning system would be unable to correctly recognize any of the digits zero to nine, for example, if they were not part of our training dataset.

The following figure illustrates the concept of a binary classification task given 30 training samples: 15 training samples are labeled as negative class (circles) and 15 training samples are labeled as positive class (plus signs). In this scenario, our dataset is two-dimensional, which means that each sample has two values associated with it: Classification for predicting class labels and Classification for predicting class labels. Now, we can use a supervised machine learning algorithm to learn a rule—the decision boundary represented as a black dashed line—that can separate those two classes and classify new data into each of those two categories given its Classification for predicting class labels and Classification for predicting class labels values:

Regression for predicting continuous outcomes
We learned in the previous section that the task of classification is to assign categorical, unordered labels to instances. A second type of supervised learning is the prediction of continuous outcomes, which is also called regression analysis. In regression analysis, we are given a number of predictor (explanatory) variables and a continuous response variable (outcome), and we try to find a relationship between those variables that allows us to predict an outcome.

For example, let's assume that we are interested in predicting the Math SAT scores of our students. If there is a relationship between the time spent studying for the test and the final scores, we could use it as training data to learn a model that uses the study time to predict the test scores of future students who are planning to take this test.

Note
The term regression was devised by Francis Galton in his article Regression Towards Mediocrity in Hereditary Stature in 1886. Galton described the biological phenomenon that the variance of height in a population does not increase over time. He observed that the height of parents is not passed on to their children but the children's height is regressing towards the population mean.

The following figure illustrates the concept of linear regression. Given a predictor variable x and a response variable y, we fit a straight line to this data that minimizes the distance—most commonly the average squared distance—between the sample points and the fitted line. We can now use the intercept and slope learned from this data to predict the outcome variable of new data:


