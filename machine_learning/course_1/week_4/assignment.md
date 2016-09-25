# Assignment Week 4

## Question 1
Compare top words according to word counts to TF-IDF: In the notebook we covered in the module, we explored two document representations: word counts and TF-IDF. Now, take a particular famous person, 'Elton John'.

**What are the 3 words in his articles with highest word counts?**

1. the
2. in
3. and

**What are the 3 words in his articles with highest TF-IDF? These results illustrate why TF-IDF is useful for finding important words.**

1. furnish
2. elton
3. billboard

## Question 2

Measuring distance: Elton John is a famous singer; let’s compute the distance between his article and those of two other famous singers. In this assignment, you will use the cosine distance, which one measure of similarity between vectors, similar to the one discussed in the lectures. You can compute this distance using the graphlab.distances.cosine function.

**What’s the cosine distance between the articles on ‘Elton John’ and ‘Victoria Beckham’?**

0.9567006376655429

**What’s the cosine distance between the articles on ‘Elton John’ and Paul McCartney’?**

0.8250310029221779

**Which one of the two is closest to Elton John? Does this result make sense to you?**

Paul McCartney

### Question 3

Building nearest neighbors models with different input features and setting the distance metric: In the sample notebook, we built a nearest neighbors model for retrieving articles using TF-IDF as features and using the default setting in the construction of the nearest neighbors model. Now, you will build two nearest neighbors models:

* Using word counts as features
* Using TF-IDF as features

In both of these models, we are going to set the distance function to cosine similarity. Here is how: when you call the function

`graphlab.nearest_neighbors.create`

add the paramater

`distance='cosine'`

Now we are ready to use our model to retrieve documents. Use these two models to collect the following results:

**What’s the most similar article, other than itself, to the one on ‘Elton John’ using word count features?**

Cliff Richard

** What’s the most similar article, other than itself, to the one on ‘Elton John’ using TF-IDF features?**

Rod Stewart

** What’s the most similar article, other than itself, to the one on ‘Victoria Beckham’ using word count features?**

Mary Fitzgerald

**What’s the most similar article, other than itself, to the one on ‘Victoria Beckham’ using TF-IDF features?**

David Beckham