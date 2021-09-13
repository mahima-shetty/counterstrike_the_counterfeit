
Designed by BootstrapMade.com
# CounterStrike the Counterfeit
![44773825-CNBC-counterfeit-drugs-cover](https://user-images.githubusercontent.com/41589522/133074591-96714bb4-9878-4cc2-83e0-e3095e4dfb43.jpg)


### Counterfeit and falsified drugs can have a serious impact upon human health. These drugs can also influence microbial resistance as well as have an effect on pharmaceutical companies’ profits and branding. Tackling counterfeit drugs is therefore an important issue which companies and governments alike are looking to combat.


These are the top aspects in observing the :
- Weight of counterfeit medicines
- MRP of the medicine originalprice and counterfeit price
- Type of Medicines
- City Tier
- Education of society
- Awareness regarding counterfeit medicines
- SideEffect Level of the medicines

***Credit: https://www.europeanpharmaceuticalreview.com/article/92194/the-impact-of-counterfeit-drugs-in-south-and-south-east-asia/***

<hr>
According to some estimates, more than 10 percent of all pharmaceuticals in the global supply chain are counterfeit. In some countries, fake pharmaceuticals account for 70 percent of all drugs in the supply chain.
</br>

In our dataset, we have good characteristics like </br>


  **Weight of counterfeit medicines**  
  Weight of the counterfeit medicines are **moderately** contributed to the EDA and model decision making. We are nearly failed to take the weight of the counterfeit medicine as primary feature to call for precision of the value. </br>
  
**MRP of the medicine originalprice and counterfeit price** <br/>
  MRP of the counterfeit medicines are **highly** contributed to the EDA and model decision making. We can see the comparable results in MRP as well as in counterfeit sales. Higher the MRP, so thus can be seen in the model decision making.<br/>
  
**City Tier** <br/>
  City Tier is the feature which shown a **very high** correlation with respect to others. It can be seen that Tier 3 cities have a high rate of counterfeit medicines sales.
  India: Indian pharmaceutical companies have suggested that in India’s major cities, one in five strips of
  medicines sold is a fake. They claim a loss in revenue of between 4% and 5% annually. The industry also
  estimates that spurious drugs have grown from 10% to 20% of the total market.
  Nigeria: Nigerian health officials estimate that 70% of drugs in circulation in the country are either fake or
  adulterated.<br/>
  
**SideEffect Level** <br/> 
  SideEffect level also has a certain level in contributing to the Analysis and model making.

# Machine Learning Model Making

</br>
Problem faced during the process.</br>

1. Oversampling</br>
 Tried doing method of Random OverSampling, Random duplicancy of records in the minority class.
 
2. Undersampling</br>
 Tried doing method of Random UnderSampling, Random deletion of records in the majority class.
 
3. Working Bias and Variance</br>
 The data was prone to high Variance and Bias. This situation is considered bad as it will affect the prediction sales.

For **Bias**  </br> K fold resampling, in which a given data set is split into a K number of sections, or folds, where each fold is used as a testing set.</br>
Bootstrapping, which involves iteratively resampling a dataset with replacement.

For **Variance**  </br>
Variance can lead to overfitting, in which small fluctuations in the training set are magnified. A model with high-level variance may reflect random noise in the training data set instead of the target function. The model should be able to identify the underlying connections between the input data and variables of the output.
</br>

The encoded variables </br>
**One Hot Encoding** - the categorical feature is not ordinal (like the Types of Medicines above)</br>


**Label Encoding** - the categorical feature is ordinal (like the Tier City above)


Counterfeit drugs not only reduce profits for pharmaceutical companies. 
Once taken by patients, falsified drugs can cause health problems and even be fatal.





Model Tuning: 
For data model, I have used Random Forest Regressor after analyzing with various ML models. 

**GridSearchCV**  

Tuning the hyperparamters  It helps to loop through predefined hyperparameters and fit your estimator (model) on your training set. So, in the end, you can select the best parameters from the listed hyperparameters.

**Why chose GridSearchCV over RandomSearch CV?**
Random search is the best parameter search technique when there are less number of dimensions. But we have good number of dimensions in hand. So in this grid Search CV, is better.


</br>
![Random Forest 03](https://user-images.githubusercontent.com/41589522/128638871-b6d1eba3-b5bf-4c28-b9a5-af7c8d36669d.gif)
***Image Credit: Tensorflow Blog***
<hr>

## Scores in Final Model 😀

~ 50% Accuracy


<hr>

## Model Done! Integration with website 😇
Heroku App deployment
<hr>

![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/41589522/128636251-60f73340-d808-4926-a27f-79571a20b8c1.gif)
