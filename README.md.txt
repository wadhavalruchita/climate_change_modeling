# Climate Change Modeling Project

This project uses sentiment analysis on over 500 user comments from NASA's Facebook page to predict user engagement (likes) based on sentiment. A **Random Forest Regressor** model is used to predict `likesCount` based on sentiment, and scenario analysis is performed to simulate how different sentiment levels impact engagement.

## Project Structure


## Setup Instructions

To run the project, follow these steps:

### Step 1: Install Python

Make sure you have **Python 3.x** installed on your system. You can download Python from the official website: [https://www.python.org/downloads/](https://www.python.org/downloads/).

### Step 2: Set Up a Virtual Environment (Recommended)

It's highly recommended to use a virtual environment to manage project dependencies. Here's how to set up a virtual environment:

### open command prompt or terminal

1. Create a virtual environment:
   ```bash
   1) python -m venv myenv        ### run this line first

   2) myenv\Scripts\activate    ### it will activate the virtual environment.

2. Install required libraries
Once the virtual environment is activated, install all necessary libraries by running:

   pip install -r requirements.txt     ### run this line

3. Launch Jupyter Notebook

    jupyter notebook        ### run this line

4. Load the model

The model has been pre-trained and saved as climate_change_model.pkl. You can use the following code to load the model and make predictions:

import joblib

# Load the pre-trained model
model = joblib.load('climate_change_model.pkl')

# Example prediction
future_data = pd.DataFrame({
    'sentiment_Positive': [1, 0],
    'sentiment_Neutral': [0, 1]
})

# Make predictions
predictions = model.predict(future_data)
print(predictions)


