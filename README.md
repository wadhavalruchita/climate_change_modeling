# Climate Change Modeling Project

This project analyzes user comments from NASA's Facebook page about climate change to predict user engagement (`likesCount`) based on sentiment analysis. The project uses a **Random Forest Regressor** model for predictions and includes scenario analysis to explore how sentiment impacts engagement.

---

## **Project Structure**

climate_change_modeling/ │ ├── climate_change_modeling.ipynb # Jupyter Notebook with project code ├── your_dataset.csv # Dataset file ├── climate_change_model.pkl # Saved machine learning model ├── requirements.txt # List of required libraries └── README.md # Instructions for running the project


---

## **Setup Instructions**

### **Step 1: Install Python**
Make sure you have **Python 3.x** installed on your computer. You can download it from [python.org](https://www.python.org/).

---

### **Step 2: Set Up a Virtual Environment (Optional but Recommended)**

Using a virtual environment ensures that the project dependencies don’t interfere with other Python projects. Here’s how to create and activate one:

1. **Create a virtual environment**:
   ```bash
   python -m venv venv

2. Activate the virtual environment:
On Windows
    ```bash
   venv\Scripts\activate


## Step 3: Install Required Libraries
Install the required Python libraries using the requirements.txt file. Run the following command:

bash
pip install -r requirements.txt

## Step 4: Resolve Path Issues
To ensure the project works without path issues:

Keep all files in the same folder:

Ensure the dataset file (your_dataset.csv), the saved model (climate_change_model.pkl), and the notebook (climate_change_modeling.ipynb) are all in the same folder.
Use relative paths in the code: The notebook is already configured to use relative paths. You should not need to modify anything if all files are in the same folder.

Set the current directory (if needed): If the project files are in a different folder, you can set the working directory in the notebook using:

python/jupytor
import os
os.chdir('path_to_project_folder')  # Replace with your project folder path


## Step 5: Run the Jupyter Notebook
Open the terminal or command prompt and navigate to the project folder:

bash

cd path_to_project_folder

#Launch Jupyter Notebook:

bash

jupyter notebook


Open climate_change_modeling.ipynb in the Jupyter interface and run the cells step by step.


##### Common Issues and Solutions
1. Missing Libraries
If you encounter a ModuleNotFoundError, make sure all required libraries are installed by running:

bash
pip install -r requirements.txt

2. Path Issues
Ensure all files (your_dataset.csv, climate_change_model.pkl, etc.) are in the same folder as the notebook.
If you need to manually set the working directory, use:
python
import os
os.chdir('path_to_project_folder')

3. Model File Not Found
If the climate_change_model.pkl file is not found, ensure it is present in the same folder as the notebook. If it’s missing, you may need to re-train the model by running all cells in the notebook.

