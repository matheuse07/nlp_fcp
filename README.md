# nlp_fcp

# **Assignment / FCP**

**0/not helpful:** less than 30% of IMDB users found movie review “i” helpful

**1/helpful:** more than 70% of IMDB users found movie review “i” helpful

## **Data and file description**

The training data (train.csv, see the download area below) contains 10,755 labeled reviews. The test data contains 5,071 reviews that are unlabeled (test.csv, see below). All the reviews included in the dataset have at least 80 votes.

File description:

- **train.csv:** your training data (N = 10,755). The first column, ‘’helpfulness_cat”, is the label of each training movie review; the second column, “imdb_user_review”, contains the text of the movie review.
- **test.csv: y**our test data (N = 5,071). The first column, “_id”, is a movie review-level identifier; the second column, “imdb_user_review”, is the unlabelled movie review to classify.
- **submission.csv:** this is the file you’re asked to populate and submit. The first column, “_id”, is the review-level identifier reported in test.csv; the second column, ‘’helpfulness_cat”, will contain your predicted class label (0 or 1) for the corresponding line in text data. Note: i) please include the exact headers "_id, helpfulness_cat" in your submission — or just used the file I make available in the download area below; ii) stick with the movie identifiers included in the column “_id” of test.csv.

---

**Download the files ⬇️ 🗂**

Available in the 'data' folder of this repo

## Guidelines

To carry out the classification task, you can use any classifier or combination of classifiers, any combination or selection of features, and either supervised, semi-supervised, or even transfer learning approaches. For example, the features may include (but are not limited to) BoW vectors, TFIDF vectors, vectors achieved with embedding algorithms, topic-to-document probabilities. In terms of estimators, you can use logistic regression, Naive Bayes Classifier, or any other estimator you think is appropriate given the nature of the task.

## **Submission**

### When / deadline

Submit your FCP via Moodle by Wednesday 20th July 2022 (4:00 PM)

### What / submission p**ackage**

The submission should comprise:

- **submssion.csv:** the first column contains movie review-identifiers, “_id”, as per test.csv (e.g., “610d01fe9a63eb113d2235ac”); the second column, “helpfulness_cat”, is the category (or label) predicted by your classifier, one of {0/not helpful, 1/helpful}
- **a 2,000-word companion report.** This document should report:
    - the various logical steps behind your classifier
    - the justification of each step — e.g., why you use a certain estimator rather than others
    - how the classifier could be improved — this is not necessary if your F1 Score = 1. 😎 🆒
- **the companion Python, Julia, or R code:** I leave the choice of one of these three languages with you. Irrespective of the language you go with, the code must be reproducible.

## Assessment

Your mark is calculated as follows:

FCP mark = 0.5 X solution effectiveness + 0.5 X clarity and organization of materials

By **solution effectiveness**, I mean a very simple thing: the [F1 Score](https://en.wikipedia.org/wiki/F-score) of your classifier, that is, the harmonic mean of precision and recall. Don’t try to overfit your model. If you do that, I’ll spot the problem and your submission will go straight to the ethics committee. 🚔 👮‍♀️👮

Regarding the ‘clarity and organization of materials’ dimension, I value it positively:

- clear and simple writing, e.g., short sentences
- concise writing, i.e., added value per word
- the use of academic references supporting the design choice of your classifier
- the use of compelling logical arguments supporting the design choice of your classifier
- evidence of critical thinking at large
- cross-references connecting the computer code with the companion report
- formatted computer code
- the use of functions and ad hoc classes
- commented computer code
