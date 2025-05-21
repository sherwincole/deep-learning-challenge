**Overview of the Analysis**

The purpose of this analysis is to create a binary classification model using deep learning techniques to predict if an organization funded by Alphabet Soup will be successful in their venture. The model utilizes a dataset of over 34,000 organizations that have received funding from Alphabet Soup, containing metadata about each organization.

**Data Preprocessing**

-   **Target variable(s) for the model:** The target variable for the model is "IS_SUCCESSFUL".
-   **Feature variable(s) for the model:** The feature variables for the model include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
-   **Variable(s) removed from the input data:** The EIN and NAME columns were removed from the input data as they are identification columns and not useful as features or targets.

**Compiling, Training, and Evaluating the Model**

-   **Neurons, layers, and activation functions selected for the neural network model and rationale:** The model consists of three hidden layers with 14, 7, and 1 neurons, respectively, and ReLU activation functions. The output layer uses a sigmoid activation function for binary classification. The structure was chosen to provide a balance between complexity and the potential for overfitting, while maintaining the ability to learn complex patterns in the data.

This model did not achieve desired accuracy of 75%. The accuracy achieved was 72.9%.

![Screenshot 2025-05-21 at 6.02.16 PM.png](blob:https://euangoddard.github.io/57f4fa41-b59b-4bfb-92d0-4932a671b35f)

In this project, we ran about 4 models. The last 3 models removed the EIN and NAME columns and with applying different neurons and layers and binning as bellow:

-   Attempt1: Use same structure but different number of neurons in each layer 100 and 50

-   Accuracy stayed the same at  72.9%

![Screenshot 2025-05-21 at 6.02.07 PM.png](blob:https://euangoddard.github.io/09a741bd-48fb-41f0-b9e1-03806065e0fe)

-   Attempt 2: Kept the same layer just dropped the epochs down to 25 

-   Accuracy increased to 73%

![Screenshot 2025-05-21 at 6.01.55 PM.png](blob:https://euangoddard.github.io/21fc562c-b97e-469b-aee7-af169d450468)

-   Attempt 3: Added more neurons 300 and 150, kept the epochs to 25 

◦  Accuracy decreased to 72.8%

![Screenshot 2025-05-21 at 6.01.43 PM.png](blob:https://euangoddard.github.io/decff75b-9f98-4190-80f0-ade43476e0a3)

**Steps taken in attempts to increase model performance:** To increase model performance, the following steps were taken:

-   Adding more neurons to a hidden layer.
-   Adding or removing hidden layers.
-   Increasing or decreasing the number of epochs in the training regimen.

**Summary**

The deep learning model did not achieve the desired performance of 75% accuracy in predicting the success of Alphabet Soup-funded organizations. Several attempts were made to optimize the model through data preprocessing and neural network structure adjustments.# deep-learning-challenge
