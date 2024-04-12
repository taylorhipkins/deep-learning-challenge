# Deep Learning Challenge Report

# Overview of the analysis: Explain the purpose of this analysis.
The purpose of this analysis was to use a deep learning model to determine the success of Alphabet Soup-funded organizations based on a provided dataset.

# Results: 
## Data Preprocessing
What variable(s) are the target(s) for your model?
The target variable in this analysis is "IS_SUCCESSFUL." 

What variable(s) are the features for your model?
The features include all the columns in the dataset except for the target variable, "EIN," and "NAME." 

What variable(s) should be removed from the input data because they are neither targets nor features?
"EIN" and "NAME"

## Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
For my first attempt, I chose two hidden layers with the first layer having nine neurons in the second layer having six neurons. The hidden layers had an activation function of relu and the output had an activation layer of sigmoid. I choose these numbers randomly to build my optimation attempts off of. 

Were you able to achieve the target model performance?
I was not able to reach 75% accuracy. All of my attempts were around 73% accuracy.

What steps did you take in your attempts to increase model performance?
I originally began by dropping the 'EIN', 'NAME', 'STATUS', and 'SPECIAL_CONSIDERATIONS' columns but realized they had higher accuracy percentages just dropping the 'EIN', and  'NAME' columns. I also changed the application types cutoff_value to 725. I began by increasing the number of hidden layers from 2 to 3 and increasing the amount of neurons to 20-25 as it is about half of the number of input features (43). After not seeing much progress in the percent accuracy in my first three optimization attempts i reduced the number of layers and the number of neurons and to 2 layers with 10 and 8 neurons respectively and got an accuracy of 73.34% accuracy. 

# Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
My final optimation attempt resulted in 73.34% accuracy with a 55.52% Loss.Utilizing a model that has stronger correlation between input and output may result in increased prediction accuracy. Using different activation features can also help the model due to the relationships within the data.


