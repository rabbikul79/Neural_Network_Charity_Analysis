# Neural_Network_Charity_Analysis

## Overview of the analysis: 
Using a mechine learning model for a non-profit foundation to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results:

### Data Preprocessing
 * What variable(s) are considered the target(s) for your model?</br>
      - IS_SUCCESSFUL Column<br/>
 * What variable(s) are considered to be the features for your model?</br>
      - All others except the target and two dropped columns<br/> 
 * What variable(s) are neither targets nor features, and should be removed from the input data?</br>
      - EIN and NAME columns<br/>

### Compiling, Training, and Evaluating the Model<br/>
  * How many neurons, layers, and activation functions did you select for your neural network model, and why?
      - There were two hidden layers:  Layer 1 included 80 neurons and Layer 2 included 30, both used the relu activation function.  The output layer used the sigmoid function.<br/>
![D2_Model](https://user-images.githubusercontent.com/85530486/141609136-4dc5eec2-6238-435e-922d-f61f98c43c1e.png)

  * Were you able to achieve the target model performance?</br>
      - The model performance was not optimal as the accuracy was 68%</br>
 ![D2_Model_Evaluation](https://user-images.githubusercontent.com/85530486/141609268-4ab81fb3-8064-4e9f-bbeb-2e91608d1204.png)

  * What steps did you take to try and increase model performance?
      - Three more attempt were made to increase the efficiency of the model</br>
        - Attempt 1 :Layer 1 increased neurons to 120 and Layer 2 to 45, both used the relu activation function</br>
  ![D3_Model_Evaluation_Attempt 1](https://user-images.githubusercontent.com/85530486/141609639-3bb9961f-7c49-48df-99f9-c8c9412ec326.png)

        - Attempt 2 :additional layer of 20 neurons was added, all three layers used the relu activation function</br>
![D3_Model_Evaluation_Attempt 2](https://user-images.githubusercontent.com/85530486/141609700-da9a9aeb-01ca-4c38-bd7b-b0f9aea8e3da.png)

        - Attempt 3 :Layer 1 and Layer 2 used the tanh activation function, and Layer 3 used the relu activation function</br>
![D3_Model_Evaluation_Attempt 3](https://user-images.githubusercontent.com/85530486/141609774-fc790e4c-2c5b-4b87-b14c-c39e2b9f13df.png)

## Summary:
None of these attempts were able to increase accuracy to 75% or higher.

* Recommendation: By removing more features or add more data to increase accuracy.  Otherwise, we could use Random Forest Classifier: a random forest algorithm will sample the data and build several smaller, simpler decision trees that try to select the best feature at every split.  How often a feature gets selected over the whole random forest model gives us an indication of how important that feature is. Each tree is considered a “weak classifier,” but when you combine them, they form a “strong classifier.”<br/>

