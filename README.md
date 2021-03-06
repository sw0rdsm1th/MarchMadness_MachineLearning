# MarchMadness_MachineLearning

March 2018 Kaggle competition. This repository represents various efforts at applying various scikit-learn packages to historical NCAA Men's Tourney data. My end bracket is posted as: 2018 bracket logreg.pdf

Requirements
---

* numpy = 1.11.1
* pandas = 0.18.1
* scikit_learn = 0.18.1

Instructions
---
1. If you have a MacBook, consider checking python version

  `python -version`

   Ensure that you have python 3 or greater installed (Although Python 2.7 works fine)

2. Follow directions below to install Anaconda package, to ultize Jupyter Notebook (perfect for data experiments in Python)

   http://jupyter.org/install

3. For each `.py` file, you will need to modify the path to your data in the form of file paths for data-v2 and data-v3 (this    was the way the data was downloaded from kaggle).

4. After opening a new notebook, type

  `python3 mmlogreg.py`

   Or some variation of:
   
  `python [name of python file].py`
   
Approach
---

1. Utilized ELO ranking method as an approach to rank any two teams in a matchup, based off of FiveThirtyEight and adopted code from another python programmer for my approach (never reinvent the wheel):

   https://fivethirtyeight.com/features/how-our-march-madness-predictions-work/
   
   Credit to Kasper P. Lauritzen:
   
   https://www.kaggle.com/kplauritzen/elo-ratings-in-python
   
   * Ingestion
   * Perform matchups
   * ELO ranking
   * Apply model

2. Next, I wrote a CSV file ingestion logic to process tourney data

3. To be filled in

4. Definition of each method....To be filled in

5. I applied the following algorithms from sklearn

   * GaussianNB from naive_bayes module
   * CalibratedClassfierCN from calibration module
   * RandomForest from ensemble module
   * KNeighbors from neighbors module
   * logarithmic regression from linear_model module
   
   
Lessons Learned
---

1. Picking the right model for the job
2. Adjusting error bounds - this depended on model type
3. Does machine learning even apply?

It's likely that this is a meta-question, or the ethic that guides the entire endeavor. Another way to ask, is machine learning even applicable to games of chance where the variables will exceed the ability for data anaylsts to accurately capture (i.e. how does one convert 'luck' to a value?) The top seed pick from my logarithmic regression model is Virginia. Univeresity of Maryland - Baltimore County changed that outcome at the start of the tournament.

4. Steps to improve the model types?

Select less models. This is a zero-sum game and likely perceptron or logarithmic regression would've done fine.
