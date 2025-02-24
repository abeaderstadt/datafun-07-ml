# datafun-07-ml
# Project 7 machine learning

## Overview

In Project 7 we'll create a guided project. There is no specification - we introduce some topics including machine learning as we work through the module. The project will include Jupyter. 

---
## **How to Install and Run the Project**
---
### **Step 1. Create a New Repo in GitHub**
 - Open your browser and log in to your GitHub account.
 - Select 'Create New Repository' from the dropdown menu, and name your repo.
 - Select the Public option so others can view your repository, and add a README.md file.
 - Click the 'Create repository' button to finalize the process.
 - Clone your repo to local using your new URL pasted into the following example command.
  - git clone https://github.com/youraccount/yourrepo
 - Create your .gitignore and requirements.txt files.
 - Run the following command from your project route directory to create your virtual environment.
  - py -m venv .venv
 - Use the following commands to add files to version control.
IMPORTANT: Replace the commit message with a clear and descriptive note about what you added or changed.
  - git add .    # stages changes, adds files to source control
  - git commit -m "Add .gitignore and requirements.txt files"    # creates a labeled snapshot of staged changes.
  - git push -u origin main    # updates the remote repository
 - Open the newly cloned folder to begin working in it by selecting 'file' 'open folder' navigate to the new repo and select 'open'.
---
### **Step 2. Activate Your .venv**
 - Before making any changes to a project, ALWAYS pull the latest changes from the remote repository on GitHub using the following command.
  - git pull origin main
 - Run the following command to activate your .venv # HINT- You MUST activate your .venv before editing a project.
  - .venv\Scripts\activate
---
### **Step 3. Install Packages Into Your Local Project Virtual Environment**
 - Ensure your .venv is active, update key packages, and install dependencies from your requirements.txt using the following commands.
  - .venv\Scripts\activate
  - py -m pip install --upgrade pip setuptools wheel
  - py -m pip install -r requirements.txt
---
## **Repeatable Project Workflow**
 Follow these steps when starting a new work session on a professional Python project.
### **1. Pull the Latest Changes from GitHub:**
  - git pull origin main
### **2. Activate the Project Virtual Environment:**
  - .venv\Scripts\activate
### **3. Install Dependencies As Needed:**
  - py -m pip install -r requirements.txt
### **4. Run Scripts as needed:**
  - py myfile.py   
### **5. Run Jupyter Notebooks as needed:**
 - Create a kernel from the virtual environment using:
 - py -m ipykernel install --user --name .venv --display-name "Python (.venv)"
 - click the kernel selector in the top-right corner of the notebook editor and choose the interpreter associated with your .venv.
 - Click on a cell and press Shift+Enter to execute it and move to the next cell.
 - Alternatively, use Ctrl+Enter to execute the current cell without moving.
 - Use 'Run ALL' to execute notebooks fully before running git add-commit-push to GitHub.
 - Save your notebook periodically to avoid losing progress. Or make sure the File / Autosave option is on.
### **6. Save your work with git add-commit-push to GitHub:**
  - git add .    
  - git commit -m "Add your unique message here." 
  - git push -u origin main  


---
# Project 7
## **Project Specifications**

For **Project 7**, we'll follow the guided projects from Chapters 10.16 and 15.4 of your textbook. Below are the steps to complete the project:

### **1. Create a New Notebook**
- Create a new Jupyter notebook in your repository called `beaderstadt_ml.ipynb`.
- In a Markdown cell at the top, add the following:
  - **Title** of your project.
  - **Author** name.
  - A **clickable link** to your GitHub project repository.

### **2. Chart a Straight Line (Part 1)**
- Follow the instructions from 10.16 (starting on page 414 in your textbook).
- Use Markdown cells to create section headings as you go along.
- Use pandas DataFrames to plot Celsius vs. Fahrenheit.

### **3. Predict Average High Temp in NYC for January (Part 2)**
- Follow the instructions from 10.16 (starting on page 416).
- Organize the notebook with these sections:
  - **Part 2 - Prediction** (second-level Markdown heading)
  - **Section 1 - Data Acquisition**: Load the NYC January high temperature data from a CSV file into a DataFrame.
  - **Section 2 - Data Inspection**: Inspect the first and last few rows of the dataset.
  - **Section 3 - Data Cleaning**: Clean up the dataset, rename columns, and adjust the date series.
  - **Section 4 - Descriptive Statistics**: Use `describe()` to calculate basic stats for the dataset.
  - **Section 5 - Build the Model**: Use the SciPy `linregress` function to calculate the slope and intercept of the best fit line.
  - **Section 6 - Predict**: Use your model to predict the average high temperature for January 2024.
  - **Section 7 - Visualizations**: Create a scatter plot with a best-fit line using Seaborn.

### **4. Predict Average High Temp in NYC for January (Part 3)**
- **Section 1 - Build the Model**: Split the data into training and testing sets using `train_test_split`.
- **Section 2 - Test the Model**: Test the model and evaluate its predictions.
- **Section 3 - Predict**: Predict the average high temperature for January 2024.
- **Section 4 - Visualizations**: Create a scatter plot with a best-fit line using Seaborn.

### **5. Add Your Insights (Part 4)**
- At the end of your notebook, add a second-level Markdown heading for **Part 4 - Insights**.
- Include your observations comparing the two methods you used in the project.

---