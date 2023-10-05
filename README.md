# deep-learning-challenge
Neural Network Report

Purpose

The primary aim of this analysis is to assess the potential success of clients who receive funding from Alphabet Soup by utilizing a neural network for predictive purposes.
Findings

Data Preparation
Target variable: Our predictive focus centers on the "IS_SUCCESSFUL" column.
Feature variables: All other columns in the dataset serve as our feature variables.
Excluded variables: The "EIN" and "NAME" columns, being irrelevant and neither targets nor features, were excluded from consideration.
Model Compilation, Training, and Evaluation
Initially, the model was designed with three layers, including two hidden layers each containing 16 neurons and an output layer. The "relu" activation function was chosen for both hidden layers as it is considered a universal starting point.
Regrettably, the desired performance target was not achieved. However, we came close, achieving an accuracy rate of approximately 73%.
To enhance the model, five adjustments were made:
The cutoff value for replacing application counts was increased from 100 to 1000.
The cutoff value for replacing classification counts was also raised from 100 to 1000.
Two additional hidden layers were incorporated, resulting in a total of four hidden layers and five layers in total.
The number of neurons in each hidden layer was increased from 16 to 100.
The number of training epochs was extended from 100 to 200.

Summary
In conclusion, the optimized learning model has produced acceptable results, with an accuracy rate of 73% and a loss rate of 63%, albeit with a slight increase from the initial model's loss rate of 56%. To further enhance the model's performance, I recommend exploring additional avenues for optimization. Given the substantial volume of data in the original CSV file (comprising over 30,000 rows), it is crucial that the model can efficiently handle such large datasets. One potential avenue for improvement could involve introducing more hidden layers with increased neuron counts, thus allowing for better feature representation and predictive power.
Additionally, considering an alternative activation function, such as the leaky ReLU function, may offer advantages. Leaky ReLU accommodates both negative and positive normalized nonlinear values, a characteristic that became apparent during the data scaling process. Despite these constructive insights, it is important to acknowledge that this model still requires further refinement before it can be confidently recommended for professional applications.