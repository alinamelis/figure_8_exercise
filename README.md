### Udacity DS Nanodegree (Disaster Response Pipeline project)

This project analyzes disaster data from Figure Eight to build a model for an API that classifies disaster messages, as well as loads results into a web app where an emergency worker can input a new message and get classification results in several categories. 

### Content:

1. ETL Pipeline Preparation.ipynb >> Jupyter notebook used as source for data processing script (data / process_data.py)
2. ML Pipeline Preparation.ipynb >> Jupyter notebook used as source for machine learning script (data / train_classifier.py)
3. data.zip >> Archive containing data necessary for analysis:
    -  disaster_categories.csv (file with categories)
    -  disaster_messages.csv (file with disaster messages)
    -  DisasterResponse.db (example of resulting database, should be removed before the scripts are run)
    -  process_data.py (data processing script)
    
4. models.zip >> Archive containing script necessary for model building
    -  train_classifier.py (machine learning script, will build and save a model)

5. app.zip >> Archive containing files necessary for web app:
    - run.py (compiles and runs web application)
    - tempates (folder with html files for the web page)


### Instructions:
1. Unpack all archives into corresponding folders. You don't need Jupyter Notebooks.
2. Delete data / DisasterResponse.db 
3. Run the following commands in the project's root directory to set up the database and model.
    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

4. Run the following command in the app's directory to run your web app.
    `python run.py`

5. Go to http://0.0.0.0:3001/


### Contributing:

Changes and suggestions for a better model are welcome. For major changes, please open an issue first to discuss what you would like to change.
