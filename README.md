<h3>Task:</h3>

This is a more recent project, done in collaboration with Hady Kotaich, Stephanie Maaz, and Simon Zouki. Our country has been experiencing unprecedented hyperinflation, and with the currency losing so much of its value so quickly, we wanted to see if we could derive meaningful relationships.
<h3>Algorithm: </h3>

Our input was mainly of two types: auto-regression statistics like rolling mean etc, and sentiments and frequencies from scraping twitter. 
After performing exploratory data analysis, we tried several machine learning models (linear regression, neural net regression, tree regresssion…) After hyperparameter optimization, we found that humble linear regression with some regularization slammed the other algorithms.
<h3>Result: </h3>

The currency ranged in value from 2000 to the dollar, to 7000 to the dollar. Our mean absolute estimation error was 45 lira per day. In comparison, the model which just predicted the previous day’s value struck a 95 error per day. This is over double the accuracy. It is impressive given the stochastic nature of the variable we are dealing with.
<h3>File guide: </h3>

Chart shows the lines for the actual rate as well as the predicted rate by our model. You can see that there is a very close match, since the error is quite small compared to the value of the lira, due to both the relative low daily fluctuation and the accuracy of our algorithm.

Table shows some comparison metrics for different predictions, including the dummy baseline and the chosen linear regression.

Phase2final and phase3final are the notebook codes used to do EDA and run different models respectively. They are fairly involved.
