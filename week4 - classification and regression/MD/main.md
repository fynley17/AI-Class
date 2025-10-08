# Classification vs Regretion

 - regression predictis <b>Continuous</b> numerical values
    - for exmple house prices temperature and student grades

 - Classification predicts Discrete, categotcal labels
    - yes/no spam/not spam

### Linier regression
 - statistical method used to model relationship between variables by fitting a straight line to the observed data
 - primary goal is to predict a continuous dependant variable Y based on independent variable X

 ![alt text](image.png)

 - Line of best fit is calculated using the method of least squares


### Logistic Regression
like linier regression but classification
 - used for <b>binary classification</b>
 - classification algorithm that predicts a probability which is mapped to discrete class.
 - type of <b>Generalised Linear Model</b> (GLM) that models the log-odds of a catagorical outcome

![alt text](image-1.png)

 - instead of modelling the response variable Y directly it models the probability P(Y=1) using the logistic function, also known as <b>Sigmoid Funciton</b>
 - the function squashes the linear output to a value which is interpreted as a probability

![alt text](image-2.png)

### Feature Scaling



### Imputation

<b>Replaces missing data and values with substituted estimates</b>

![alt text](image-3.png)

### Ensemble Methods

ML techique where <b>predictions from multiple models are combined to produce a single, superior prediction</b>.

 - core principle is that a diverse committee of models will outperform any individule member

#### Decision Trees

![alt text](image-4.png)

 - in a sense it is a flowchart
 - always supervised learning
 - predicts valuse of target variable by learning simple decision rules inferred from data features
 - process of building tree is <b>Recursive Partitioning</b>
 ![alt text](image-5.png)
 - goal is to choose a split that results in the largest reduction in impurity for classification this is commonl done with Gini impurity <br>![alt text](image-6.png)

### Random forest
 - Builds hundreds of decision trees and combines their predictions
 - Main weakness of decision tree: <b>overfitting</b>
 - <b>trained on a different random sample of the data
 - reduces variance</b> makes the model more stable by averaging ou the individual tree errors
 - <b>decorrelates the trees</b> forcing them to be diverse and prevent the model from relying too heavily on a few dominant feature.
![alt text](image-8.png)
![alt text](image-7.png)

### Gradient boosting

 - Ensemble ML technique that builds a strong predictive model by sequentially adding weak learner models.
 - each new model is <b>trained to correct errors made by the combination of the previous model.</b>
 - the idea is to combine many simple models into more powerfule models
 - random forest builds models in parallel, gradient boosting builds them sequentially
 ![alt text](image-9.png)
 ![alt text](image-10.png)

### Gradient vs forest
#### Gradient
 - need <b>highest possible accueacy</b>
 - spend time <b>tuning yperparameters</b>
 - <b>computational resorces</b> for a potentially longer time

#### Forest
 - <b>strong, reliable baseling model quickly</b>
 - <b>easy to impliment and tune
 - concerned about overfitting</b> and need a stronger model
 - take advantage of <b>parallel processing</b> to speed p training 

### eXtream Gradient Boosting
<b>XGBoost is widley considered one of the most ppowerful and effective predictive algorithms avalible</b>

### Support Vector Machines
 - <b>finds an optimll hyperplane to separate data points into different classes
 - </b>effectiveness depends heavily on problem
 - more modden algorithms provide better performance and training times
 - still important anre now a bit obsolete

### Stacked Generalisation
 - EML that combines predictions from multiple models to generate a new often more powerful final prediction.
 - uses a "meta-model" whosejob is to learn the best way to combine the outputs of several "base Models".
 - extreamly effeective
 - prodcing some of most accurate and powerful predictive models avalible but complex to impliment and slow to train.<br>
 ![alt text](image-11.png)![alt text](image-12.png)

### Model parametes
<b> these are what the models learn</b>
 - these are <b>values that the model learns on its own</b>
 - dont see them manually

#### Hyperparameters
 - very important to have and what you pick
 - they are the config settings set before process begins
 - control how model learns
 they are not learned from data they are external to it 
 - the choice of them has a significant impact on model performance incorrectly set could lead to over and under fitting

![alt text](image-13.png)
#### hyperparameter tuning
 - process of systematically <b>searching for the combination of hyperparameter values that results in the best performance

![alt text](image-14.png)

#### hyperparameters w/ Combinatorics
 - <b>hyper parameter tuning is a search problem</b>
 - you have a <b>discrete set</b> if hyperparameters and eachhas a range of possible values
 - <b>trying to find the single optimal combination</b> ou of vast final set of possibilities that maximises a specific <b>objective function</b> (fitness function)

 ![alt text](image-15.png)
 ![alt text](image-16.png)