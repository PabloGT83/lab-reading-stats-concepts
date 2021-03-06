<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Lab | Reading About Statistic Concepts

## Introduction

In the future, you will need to understand deep statistical concepts by reading technical articles. As a training for that, it is interesting to start from here. Also, as we have limited time, this is a way to have some self guided learning to understand everything better and have a wider knowledge.

This week you will find some questions here that you will need to answer by documentating yourself. So you will do a different PR for each question (you are meant to answer the questions in different days). Don't hesitate to write as many text as you need and push images if you need them.

Remember for this lab: there is a right answer. But there is no perfect way to explain it (except for in a mathematical way, but this is another story).

## Challenges

### Challenge 1: What is the difference between expected value and mean?
You know both concepts but, is there a difference? Are they synonims? Start investigating. 



As a good reference (once you have looked for some information) you have   [this](http://expected.news/value2) article.

ANSWER:

The expected value is more related with ideal scenarios in terms of probabilistics. So as per the article, the expected value is the average probable value according to the ideal distribution of probabilities. 

But the mean is referred to the sample of population itself. So after conducting the experiment, lets say of rollind the dice, we will have an obtained mean of the values for that sample.

The same apply to an ideal model and its expected value vs the sample obtained for the reality of the experiment, game or process. 

In the absolute long term, expected


### Challenge 2: What is the "problem" in science with p-values?
We have told you that a lot of scientifical investigations are based on p-values. The last week, Nature magazine published [an article](http://nature.social/statistical4) regarding the problem. Start digging on it!

Don't hesitate to use more articles if you want to :)

ANSWER:

The p-value is a meaure to reject the null hipothesis. It means that normally H0 is built in a way that allows to create a double negation so something cannot be discarded. 

So if we are checking the effect of a new vaccine for Cov19, our H0 would be:

H0: the vaccine does not influence the chance of contagion
H1: the vaccine does influence the chance of contagion. 

So a low p-value would allow us to reject H0, there is no no-influence, but DOES NOT ALLOW to confirm H1. 

In case of experiments were samples are limited, are focused on human behaviour (like economics) etc.. slightly high p-values are rejecting then null hipothesis and people are thereby denying the potential no no-relationship. 

But that has a lot to do with experimental design and dependencies or spurian correlation in the model. Thereby we may have a non statistical significance in our formula but a model that is totally ok to be used for business or economic decisions. 

It is harder to accept that discussion for natural sciences, as in that case the sample and population shall be revisitied as well as the experimental set up. 



### Challenge 3: Applying testing to a specific case: A/B testing.
A/B testing is a widely used tool to understand differences between two samples. It is a way to measure the impact of something we did: 
* A marketing campaign.
* A new feature in our application. 
* A new design in our application.
* A different flow in the User Experience flow.

To do this, is very important first to design our experiment. 
* We need to know how we are measuring the impact. If people has the behaviour we want with this new implementation.
* We choose a control group (people who doesn't have/see the new change) and the group which will see the new change. 
* We think about how much data do we need.
* We measure the difference between them.

One example:
Our application has a lot of mini-games. We want people to reach the games that we think are the best but the behaviour is not the expected, they don't reach them.

So we call a designer and after a lot of work he shows us a new design for our application: we will add a button specific for that kind of games inviting the users to click on it:

*Click here to discover cool games!*

We think it will work but can we be sure? So instead of implementing this new button for all users, we implement it for 10% and we compare the results with the users that didn't have it. Is there a significant difference? Is our button working?

Read more about A/B testing with a couple of examples:

[Another example about Netflix here](http://select.video/artwork4)

[What happened to Basecamp](http://millions.social/tested7)

[An example with Python](http://math.social/tested3)

[A cool general explanation](http://arts.show/tested7)

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)

ANSWER:

A/B testing is an industry meme of bringing ANOVA ur Multivariant ANOVA to realms outside of natural science into marketing/economics. 

I am fully familiar with ANOVA and happy to apply on python models, looking forward to it. 

Basically it can be used for instance with customer accesing the self service portal of our company and checking the average time spent in the portal & number of actions self-completed against the different designs. 

In general we need to check the 2 populations (or n, if we are doing A/B/n) share the same distribution. If they do share it, we need to check on the mean and variance of the groups push into the different categories.

Thereby following a clasical ANOVA. 

## Deliverables
You need to submit a markdown file with the answers to the questions above. You can create a new `.md` file or directly edit the `README.md`.

## Submission
Upon completion, add your deliverables to git. Then commit git and push your branch to the remote.
