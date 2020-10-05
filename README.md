# Disaster Response Pipeline

Creating a machine learning pipeline to categorize real messages send during disaster events.

## Table of Contents

1. [Instructions](#start)
2. [What's Included](#files)
3. [Important Files](#licensing)
4. [Student Notes](#licensing)

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

### Whats Included:
Here's the file structure of the project:

```
- app
| - template
| |- master.html  # main page of web app
| |- go.html  # classification result page of web app
|- run.py  # Flask file that runs app

- data
|- disaster_categories.csv  # data to process 
|- disaster_messages.csv  # data to process
|- process_data.py
|- InsertDatabaseName.db   # database to save clean data to

- models
|- train_classifier.py
|- classifier.pkl  # saved model 

- README.md
```

 
### Important Files:
The input files are kept in data folder, and they are disaster_categories.csv and disaster_messages.csv.
1. Disaster_messages contain id, the translated message and the original message
2. Disaster_categories contain id along with the associated categorization

data/process_data.py: The ETL pipeline used to process data in preparation for model building.

models/train_classifier.py: The Machine Learning pipeline used to fit, tune, evaluate, and export the model to a Python pickle (pickle is not uploaded to the repo due to size constraints.).

app/templates/*.html: HTML templates for the web app.

run.py: Start the Python server for the web app and prepare visualizations.

### Student Notes:
My GitHub link: https://github.com/cenkakturk?tab=repositories
