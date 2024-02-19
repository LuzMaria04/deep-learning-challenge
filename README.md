# deep-learning-challenge
Module 21

# Overview of the analysis: Explain the purpose of this analysis.
**The purpose of this analysis is to develop a deep learning model using TensorFlow and Keras to predict the success of funding applications for Alphabet Soup, a nonprofit organization. The dataset used for this analysis is from charity_data.csv, and the target variable is "IS_SUCCESSFUL," indicating whether the funding application was successful.

# Data Preprocessing
- Removing columns “EIN” and “NAME”.
- Binning the “APPLICATION_TYPE” based on the count of number applications, then choosing the 
- “APPLICATION_TYPE” based on those with greater than 500.
- Binning the “CLASSIFICATION” based on the count of number applications, then choosing the 
- “CLASSIFICATION” based on those with greater than 100.
- Convert categorial data to numeric with ‘pd.get_dummies’.
- Split the data into features and target arrays. Our target array is the column “IS_SUCCESSFUL”.
- Splitting the dataset into training and testing datasets.
- Using StandardScaler to scale the data.

## Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model, and why? I created four models the first two models had to 2 layers with a diiferent in neureons and seconds. One consiseted of 30 while the other of 80, both models had an accuracy of 73.0% both below the 75% threshold. The numbers of layers was increased to 3 layers, 10 neurons for first, 20 for the second, and 30 for the third. And for the fourth model I went back to 2 layers but increased the # of neurons to 300 for the first layers and 100 for the second. The accurarcy stayed constant. Therefore the last model increased the number of layers to 4, 10 neurons for the first, 20 for the second and 30 for both the third and fourth layers. The accurarcy dropped to 72.7%

3. Were you able to achieve the target model performance?
  - I was not able to achieve the target model perfromnce.

5. What steps did you take in your attempts to increase model performance?
 - Increasing the layers and adjusting the neurons had little effect in obtaining the target accuracy of 75%. Additionally, to improve the deep learning model's performance, I would ensuring proper data cleaning, exploring alternative algorithms, identifying feature importance, addressing bias and outliers, and applying data binning techniques. This can enhance the model's ability to capture relevant patterns and reduce noise, ultimately improving accuracy in the classification problem.
