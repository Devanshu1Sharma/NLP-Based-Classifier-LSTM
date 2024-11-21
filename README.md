NLP Complaint Categorization Model


Problem Statement

With a high volume of complaint data, manually categorizing each case based on parameters such as victim involvement, fraud type, and other unique details is challenging and time-consuming. This project provides a solution by building an NLP model that classifies complaints based on these factors, allowing for efficient organization and prioritization in fraud investigations. 


Solution Approach 
A hybrid methodology was employed, combining robust data preprocessing, exploratory data analysis (EDA), and a Deep Learning Long Short-Term Memory (LSTM) model for effective complaint classification.


Documentation Report
The dataset consists of complaints categorized into multiple types of cybercrimes. A Confusion Matrix was used to visualize the distribution of categories, providing insights into the volume of data for each category and highlighting any class imbalance.
The "Confusion Matrix" image shows the distribution of the different crime categories in the dataset. The matrix displays the count of each crime type, providing a visual overview of the data. 
![image](https://github.com/user-attachments/assets/1857fdfe-7f7a-4b6a-8660-d9d38dcb4023)


Data Preprocessing 
Text data preprocessing is a critical step for ensuring model performance. The following steps were executed:
•	Normalization: Converted text to lowercase and removed special characters.
•	Tokenization: Split text into individual tokens (words).
•	Stopword Removal: Filtered out common but uninformative words like "and," "the," etc.
•	Stemming: Reduced words to their root forms using a custom clean_and_stem function to ensure uniformity.


Exploratory Data Analysis (EDA) 
Two key performance plots were generated during the model training phase:
1.	Accuracy Over Epochs:
o	Training accuracy started at 0.9297 and improved to 0.93 (93%).
o	Validation accuracy remained consistent, fluctuating around 92%.
2.	Loss Over Epochs:
o	Both training and validation losses decreased over epochs, indicating effective learning.
These visualizations confirmed the model's steady improvement in performance without overfitting.


Model Architecture 
The model was built using TensorFlow's LSTM framework, with the following components:
•	Input Layers:
o	input_ids and attention_mask for handling tokenized text inputs.
•	Embedding Layer:
o	Leveraged TensorFlow’s tokenizer for sequence processing.
•	Hidden Layers:
o	Dense layers with dropout regularization to prevent overfitting.
•	Output Layer:
o	A softmax-activated dense layer to predict the probabilities of complaint categories.


Model Evaluation 
Evaluation metrics were derived from the Classification Report, which showcased precision, recall, F1-score, and support for each category.
The "Classification Report" image shows the model's performance metrics, including precision, recall, f1-score, and support for each complaint category. The model achieves high performance, with most categories having precision and recall values above 0.85
![image](https://github.com/user-attachments/assets/7313fa91-03c7-4884-96ae-772ed2baa286)
Based on the information provided , the NLP model appears to have very high accuracy in categorizing the different types of cyber crimes and complaints. 
Key observations: 
1. Precision: 
The model achieves a very high precision score of 0.99 for "Any Other Cyber Crime" and 0.96 for "Child Pornography CPChild Sexual Abuse Material (CSAM)". This indicates that the model is able to classify these categories with a high degree of accuracy. 
2. Recall: 
The recall scores are also quite high, with 0.93 for "Any Other Cyber Crime" and 0.99 for "Child Pornography CPChild Sexual Abuse Material CSAM". This means the model is able to correctly identify a large proportion of the instances in these categories. 
3. F1-Score: The F1-score, which combines precision and recall, is 0.96 for "Any Other Cyber Crime" and 0.98 for "Child Pornography CPChild Sexual Abuse Material (CSAM)". These scores suggest the model is performing well in terms of both precision and recall for these categories. 
4. Support: The "support" column indicates the total number of instances for each category in the dataset. This provides context for interpreting the other metrics, as categories with more instances will generally have more robust performance. 
Overall, the model seems to have strong performance, with high precision, recall, and F1-scores for the majority of the complaint categories. This suggests the NLP approach adopted in this project is effective in accurately classifying the different types of cyber crimes and complaints. 
![image](https://github.com/user-attachments/assets/fd6534ea-29f1-415f-9599-373c8cffcd90)


Conclusion 
The NLP Complaint Categorization Model is an efficient solution for automating the classification of complaints based on parameters like victim involvement and fraud type. Leveraging advanced preprocessing, EDA, and a well-designed LSTM model, this project achieved remarkable precision, recall, and F1-scores.
This innovation promises to significantly enhance fraud investigation workflows by providing faster and more reliable categorization, ultimately contributing to streamlined operations and better resource allocation.
![image](https://github.com/user-attachments/assets/2a962a91-edaf-4df1-81d4-2d62cc4df285)
![image](https://github.com/user-attachments/assets/4578cc2e-00c2-424b-8339-1ca7b63962cc)
 
 



