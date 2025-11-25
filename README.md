# AgriFertilizer-Recommandation
A user-friendly web app built with Streamlit to recommend the best fertilizer based on soil parameters. It utilizes a trained TensorFlow model to predict the optimal fertilizer and suggests specific products.

## Table of Contents :-
1.Installation  
2.Usage  
3.Project Structure  
4.Model Training  
5.Result


## Installation :-  
To run this application locally, follow these steps:  
Clone the repository
Install the required dependencies 

## Usage :-  
To start the application, run the following command : streamlit run app.py  
This will open a new tab in your default web browser with the Fertilizer Recommendation System.  

## Features
**Soil Nutrient Analysis :** Accepts quantitative input for calcium, magnesium, potassium, sulfur, nitrogen, lime, carbon, phosphorus, and moisture to evaluate soil health.
**Automated Fertilizer Recommendation:** Uses a trained machine learning model to predict the most suitable fertilizer type based on the soil parameters provided.
**User-friendly Interface:** Streamlit-based app enables easy input and immediate results for farmers, agronomists, or students without coding experience.
**Intelligent Label Encoding and Scaling:** Preprocesses inputs using standardization and label encoding for consistent model predictions.
**Supports Multiple Fertilizer Types:** Can classify and suggest a range of fertilizer options, such as Potassium sulfate, Superphosphate, complex blends, and more.
**Fast Real-time Results:** Provides instant fertilizer recommendations after user submits soil details.
**Expandable Dataset:** Model can be retrained with new or larger datasets for improved accuracy and adaptability.

## Technology Stack
**Python:** Primary programming language for model training, backend logic, and application scripts.
**Pandas & NumPy:** Data loading, manipulation, and efficient numerical processing.
**scikit-learn:** Feature scaling, label encoding, and train-test splitting for machine learning workflows.
**TensorFlow & Keras:** Building, training, and saving neural network models for classification.
**Joblib:** Serialization of preprocessing objects like scalers and label encoders for reliable inference.
**Streamlit:** Interactive web framework for rapid deployment of the user interface and real-time recommendations.
**CSV Data Format:** Stores and organizes soil nutrient and fertilizer type information for training and predictions.

## Enter Soil Parameters :-  
In the application, you'll need to enter the following soil parameters:  
Ca (Calcium)  
Mg (Magnesium)  
K (Potassium)  
S (Sulphur)  
N (Nitrogen)  
Lime  
C (Carbon)  
P (Phosphorus)  
Moisture  
Once all parameters are entered, click the "Recommend" button to get the fertilizer suggestion.  

## Project Structure :-  
The main components of this project are:  
app.py : Contains the Streamlit application code.  
model.py : Contains the model training code.  
fertilizer_model.h5 : Pretrained model file.  
scaler.pkl : Scaler used for preprocessing.  
label_encoder.pkl : Label encoder used for encoding class labels.  

## Model Training :-  
If you need to retrain the model, follow these steps:  
Load the dataset : Ensure you have a CSV dataset named FertPredictDataset.csv with appropriate features and class labels.  
Run the model training script : python model.py  
Save the trained model and preprocessing tools: The script will save the model as fertilizer_model.h5, and the preprocessing tools as scaler.pkl and label_encoder.pkl.  

## Result :-  
The AgriFertilizer Recommendation System was evaluated on its ability to accurately recommend fertilizers based on soil properties, crop type, and environmental conditions.

## Contributing
We welcome contributions to improve and expand this fertilizer recommendation system!
Fork the Repository: Click "Fork" to create your personal copy of the project.
**Clone Your Fork:** Download it to your machine using
git clone <your-fork-url>
**Add Your Changes:** Update code, models, or documentation as needed. Suggested improvements include model accuracy, new features, user interface design, or additional fertilizer classes.
**Pull Request:** Submit your changes via a pull request. Please clearly describe what you changed and why.
**Testing:** Ensure your changes do not break existing functionality. Test your workflow before submitting.
**Discussion & Suggestions:** Feel free to open Issues for bug reports, feature ideas, or questions.

