# deep-learning-challenge
Deep Learning Challenge for UofR data bootcamp

Overview of the analysis: Explain the purpose of this analysis.
- The Purpose of this analysis was to help automatically select applicatnts for funding who have the best chance of success in their ventures. This would be exceptionally useful if you were working for a Venture Capital firm or another type of investing body. 

Results: 
Data Preprocessing

What variable(s) are the target(s) for your model?
  - The main variable that was the target for my model was the IS_SUCCESSFUL column which indicates if the money was used effectively. 
What variable(s) are the features for your model?
  - All other columns minus the EIN and NAME were used, since those two columns were merely identification columns and would not impact the data one way or another. 
What variable(s) should be removed from the input data because they are neither targets nor features?
  - Like mentioned previously, EIN and NAME were removed, but looking back, the column SPECIAL_CONSIDERATIONS potentially could have been dropped as well since it was only a boolean Yes/No column and didn't add anything to the evaluation. 
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - For the first iteration of the model, I used 3 total layers. I figured this would be a good starting point. I only made changes to this later on in iteration 3 of the model because I didn't want to change too many things between iterations, making it more difficult to find what to change to find the most benefit. 
Were you able to achieve the target model performance?
  - I was NOT able to achieve the target performance, all the models hovered just over 73%, with the first model being the most successful at 73.06%
What steps did you take in your attempts to increase model performance?
  - I attempted to further bin the Application_Type column to see if it would provide benefit to be further binned, it did not provide any noticable benefit. On the third attempt, I changed the numebr of layers to see if it would have a benefit, again, it had no discernable benefit.
  - For Future iterations, dropping the SPECIAL_CONSIDERATIONS column would be a benefit, as well as running a KerasTuner function to determine the optimal number of hidden layers and nodes to get the best results. 
