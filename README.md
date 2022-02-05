# Disaster Response Pipeline Project
In this project, we create a machine learning model to classify messages into several categories, messages received from various sources during a crisis and labeled in many sectors such as medical issue, rescue, and so on. The goal of this research is to develop a model based on this data that will aid in determining what support messages should be communicated to various helping departments in the future. To categorize messages, we utilized a multi-output classifier and a random forest classifier. After creating a classifier, we used Flask to create a web app that allows us to enter a message and receive categorization results.
### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Go to `app` directory: `cd app`

3. Run web app: `python run.py`
### File Structure:
1.App folder including the templates folder and "run.py" for the web application
2.Data folder containing "DisasterResponse.db", "disaster_categories.csv", "disaster_messages.csv" and "process_data.py" for data cleaning and transfering.
3.Models folder including "train_classifier.py" for the Machine Learning model.
4.README file
