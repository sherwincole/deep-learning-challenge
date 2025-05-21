**Overview of the Analysis**

The purpose of this analysis is to create a binary classification model using deep learning techniques to predict if an organization funded by Alphabet Soup will be successful in their venture. The model utilizes a dataset of over 34,000 organizations that have received funding from Alphabet Soup, containing metadata about each organization.

**Data Preprocessing**

-   **Target variable(s) for the model:** The target variable for the model is "IS_SUCCESSFUL".
-   **Feature variable(s) for the model:** The feature variables for the model include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
-   **Variable(s) removed from the input data:** The EIN and NAME columns were removed from the input data as they are identification columns and not useful as features or targets.

**Compiling, Training, and Evaluating the Model**

-   **Neurons, layers, and activation functions selected for the neural network model and rationale:** The model consists of three hidden layers with 14, 7, and 1 neurons, respectively, and ReLU activation functions. The output layer uses a sigmoid activation function for binary classification. The structure was chosen to provide a balance between complexity and the potential for overfitting, while maintaining the ability to learn complex patterns in the data.

This model did not achieve desired accuracy of 75%. The accuracy achieved was 72.9%.
![Screenshot 2025-05-21 at 6 02 16 PM](https://github.com/user-attachments/assets/358b9c04-c091-4368-9c79-85bf655ddf4c)



In this project, we ran about 4 models. The last 3 models removed the EIN and NAME columns and with applying different neurons and layers and binning as bellow:

-   Attempt1: Use same structure but different number of neurons in each layer 100 and 50

-   Accuracy stayed the same at  72.9%

![Screenshot 2025-05-21 at 6 02 07 PM](https://github.com/user-attachments/assets/2595582d-30e8-42b7-8369-aa1d3eee3250)


-   Attempt 2: Kept the same layer just dropped the epochs down to 25 

-   Accuracy increased to 73%
![Screenshot 2025-05-21 at 6 01 55 PM](https://github.com/user-attachments/assets/34f3d6ec-a865-4389-abff-fc0e0ad98504)


-   Attempt 3: Added more neurons 300 and 150, kept the epochs to 25 

◦  Accuracy decreased to 72.8%

![Screenshot 2025-05-21 at 6 01 43 PM](https://github.com/user-attachments/assets/d3d25117-0117-47fc-a2a0-48d6c87d8204)


**Steps taken in attempts to increase model performance:** To increase model performance, the following steps were taken:

-   Adding more neurons to a hidden layer.
-   Adding or removing hidden layers.
-   Increasing or decreasing the number of epochs in the training regimen.

**Summary**

The deep learning model did not achieve the desired performance of 75% accuracy in predicting the success of Alphabet Soup-funded organizations. Several attempts were made to optimize the model through data preprocessing and neural network structure adjustments.# deep-learning-challenge
