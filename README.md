# DS-9 Materials

Extra course materials for data science cohort 9.

## 2025-03-14

Two extra items for tonight:

1. [Bag of words naive Bayes classifier](https://github.com/gperdrizet/ds9-course-materials/blob/main/resources/bag_of_words_naive_bayes.md): Explination of how bag of words modeling with a naview Bayes classifier works using a simple toy example.
2. [Classifier threshold tuning](https://github.com/4GeeksAcademy/gperdrizet-diabetes-prediction/blob/main/src/04-decision_threshold_tuning.ipynb): Demonstration of classifier decision threshold tuning using the diabetes prediction project dataset and models.

## 2025-03-10

Here is a link to the Adaboost meta-estimator in SciKit-learn: [`AdaBoostClassifier()`](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html). Adaboost is a sequential ensemble technique very similar to gradient boosing, but it can be used with any SciKit-learn model that supports class weighting (ex: logisic regression, random forest, etc.).

## 2025-03-07

Here are the two SciKit-learn meta-estimators for implementing your own ensemble methods:

1. [`BaggingClassifier()`](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.BaggingClassifier.html). Takes a classifier model as an argument. Trains n copies of that model on subsets of the data. Used to make your own 'forest' with any classification model type.
2. [`VotingClassifier()`](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.VotingClassifier.html). Takes a list of classifier models and aggregates their predictions via majority voting. Can be used to create ensembles of more than one model type.

Also worth a read - the original paper describing random forests: [Ho, T.K. (1995) Random Decision Forest](https://github.com/gperdrizet/ds9-course-materials/blob/main/resources/articles/Ho_random_decision_forests_1995.pdf). A little math heavy, but short and to the point. It does an excellent job explaining the motivation behind random forests and serves as a great primer on ensemble methods in general.

## 2025-03-05

**Updated**: project boilerplate repository. Use this to fork your projects (or fork from my MVP repo): [4Geeks_datascience_project](https://github.com/gperdrizet/4Geeks_datascience_project)

Here are the links for the cross-validation resources from SciKit-learn we discussed in class tonight:

1. [Cross-validation: evaluating estimator performance](https://scikit-learn.org/stable/modules/cross_validation.html)
2. [`cross_val_score()`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_val_score.html)

## 2025-02-24

Started list of links for 'MVP' notebooks. See [MVP_notebooks.md](https://github.com/4GeeksAcademy/gperdrizet-ds9-materials/blob/main/MVP_notebooks.md) page above.

## 2025-02-14

Added some extra information about useful statistical tests used during the Air BnB data preprocessing project. Look in the `resources` directory at [statistical_tests.md](https://github.com/4GeeksAcademy/gperdrizet-ds9-materials/blob/main/resources/statistical_tests.md)

## 2025-02-12

See the new resources directory for some directions on how to think about EDA effectively: [EDA guidelines](https://github.com/4GeeksAcademy/gperdrizet-ds9-materials/blob/main/resources/EDA.md).

## 2025-02-05

Here is the link to the patched fork of the Connecting to a SQL Database Project Tutorial for tonight:

1. [Connecting to a SQL Database Project Tutorial](https://github.com/4GeeksAcademy/gperdrizet-connecting-to-a-sql-database-project)

The issue was an out-of-date SQLAlchemy version, due to a recent major release of the library. This caused sample code provided in the project repository to break. It would be possible to re-write the code to comply with the new version, but instead I pinned the older version of SQLAlchemy so the project would continue to function as written. This type of thing is common in data science DevOps and in software development in general. Here are some relevant links that explain the situation:

1. [SQLAlchemy 2.0 - Major Migration Guide](https://docs.sqlalchemy.org/en/20/changelog/migration_20.html)
2. [BUG: Pandas 2.2 breaks SQLAlchemy 1.4 compatibility](https://github.com/pandas-dev/pandas/issues/57049)
3. [Semantic Versioning 2.0.0](https://semver.org/)
4. [My pull request for the patch](https://github.com/4GeeksAcademy/connecting-to-a-sql-database-project-tutorial/pull/30)

## 2025-01-31

DS-7 final project repositories:

1. [Natural Disasters](https://github.com/4GeeksAcademy/natural_disasters)
2. [Fantasy Sports](https://github.com/4GeeksAcademy/fantasy_sports_assistant)
3. [Breast Cancer Diagnosis](https://github.com/4GeeksAcademy/breast_cancer_diagnosis/tree/main)

## 2025-01-29

SciPy's implementation of the statistical tests for tonight's hypothesis testing exercises:

1. [T-test](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html)
2. [ANOVA (also called the F-test)](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.f_oneway.html)

## 2025-01-22

Three great sources of information about any package or library we use in Python are: GitHub, PyPI, and the library documentation. Here are two example libraries we will use a lot:

### SciPy

Core scientific/technical computing utilities in Python. Was originally written as a standardized set of numerical operation on top of the then new 'numeric array data structure' (which later became NumPy) in 2001.

1. [SciPy GitHub Repo](https://github.com/scipy/scipy)
2. [SciPy PyPI page](https://pypi.org/project/scipy/)
3. [Official SciPy documentation](https://docs.scipy.org/doc/scipy-1.15.0/index.html)

### SciKit-Learn

'SciKit' originally meant 'SciPy ToolKit' i.e. an extension to the SciPy library. Focused on machine learning and data science. Was originally written around 2010 as part of Google Summer of Code.

1. [SciKit-Learn GitHub Repo](https://github.com/scikit-learn/scikit-learn)
2. [SciKit-Learn PyPI page](https://pypi.org/project/scikit-learn/)
3. [Official SciKit-Learn documentation](https://scikit-learn.org/stable/)

## 2025-01-17

1. [Oh my git!](https://ohmygit.org/). Open source, graphical git game with commit graph visualization. Much better than the Git Interactive Exercises provided on 4Geeks.
2. [git-demo-parent](https://github.com/4GeeksAcademy/gperdrizet-git-demo-parent). The GitHub repository we made and contributed to during the in-class demo.

## 2025-01-15

Here are some of the resources about optimizers and gradient descent we looked at in class:

1. [2024 Nobel Prize in Physics](https://www.nobelprize.org/prizes/physics/2024/popular-information/). Hinton's contribution was work on *backpropagation* - a gradient estimation method that allowed neural networks to be trained (both the 'popular' and 'advanced' information tabs on this page are highly worth a read).
2. [Adam: A Method for Stochastic Optimization](https://arxiv.org/abs/1412.6980). The scientific paper describing the popular and widely used ADAM optimizer. **Highly** technical/theoretical & extremely dense. Don't expect to fully understand this one - but it's interesting/fun to look at (Note the year and the first author's affiliation).

## 2025-01-13

Here are the links to the official documentation pages for Pandas and Matplotlib:

1. [Pandas - Python Data Analysis Library](https://pandas.pydata.org/)
2. [Matplotlib — Visualization with Python](https://matplotlib.org/)
