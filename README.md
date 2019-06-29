## My solution to Instant Gratification

I ranked 360th (TOP 20%) in the [Instant Gratification on Kaggle platform](https://www.kaggle.com/c/instant-gratification/leaderboard). In "Instant Gratification" competition, we are building 512 models where each model's train data has approximately 512 rows and 40 columns. With 40 variables, a quadratic model would like more rows. With pseudo labeling, we can get an additional 400+ rows of training data and increase CV and LB score. 

**How it works?** QDA works by using points in p-dimensional space to find hyper-ellipsoids. With more points, QDA can better estimate the center and shape of each ellipsoid (and consequently make better preditions afterward).
Pseudo labeling helps all types of models because all models can be visualized as finding shapes of target=1 and target=0 in p-dimensional space. More points allow for better estimation of shapes.

P.S. This competition is a low-stakes, trial-run introduction to Kaggle Team new synchronous KO implementation. Kaggle want to test that the process goes smoothly and gather feedback on our experiences.

## In this repository you can find:
* `qda_and_pseudo_labeling.ipynb` - notebook with pseudo labeling and training Quadratic Discriminant Analysis models
