# Overview
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. 

# Results
Neural Network Model:
- Accuracy: 73.87%
- Loss: 54.49%

  -- Data Preprocessing
    - Previously successful ventures are the target variable for this model.
    - Application type, affiliation, classification, use case, organization, income amount, and ask amount are all features for this model.
    - The EIN, name, status, and special considerations variables should be removed from this model as neither are targets or features.
    ![image](https://github.com/user-attachments/assets/ccb503bf-1014-4420-bafb-e28bbe1c3c57)

    ![image](https://github.com/user-attachments/assets/268fb4de-4a9f-4313-aa6c-1f3e146d5969)
  
  -- Compiling, Training, and Evaluating the Model
    - The neural network model included 5 hidden layers with 63 neurons and two activation functions. With 42 input features a higher number of neurons was selected for the first hidden layer. More layers were added to slowly reduce the number of neurons until the output was reached. Leaky ReLu activation was chosed for it's ability to facor in some negative inputs with sigmoid being used for the output layer. Epochs were increased to 200 to give the model more opportunities to learn and self-correct.
    - Target performance was not achieved.
    - To increase model performance, the status and special considerations variables were removed as they did not add any value to the dataset. The number of hidden layers and neurons within the layers were adjusted in an     attempt to increase accuracy but failed to do so. Activation type was also adjusted but no significant change was observed.
    ![image](https://github.com/user-attachments/assets/9e1755f9-decd-4d70-a88e-96b05123f093)

    ![image](https://github.com/user-attachments/assets/404a57ae-6062-40d9-b2d0-504283bd9fbf)

    ![image](https://github.com/user-attachments/assets/80d1fc87-23b9-45e6-bb31-f3633906cb3c)

# Summary
The neural network model predicts whether applicants will be successful if funded by Alphabet Soup with 73.87% accuracy. While this indicates the model performs reasonably well, there is room for improvement, and exploring different models may help to improve results. Gradient Boosting Machines (GBMs) are effective for classification problems with structured data or Random Forest which is known fore it's bability to handle a large number of features. 

    
