
## Ronaldo_Messi Stats ETL Project
![ETL](https://github.com/JulienAganze/Ronaldo_Messi_Project/blob/master/graph.png)
### Aim of the project
The aim of this project is to explore the entire ETL(Extract Trasnform Load ) worflow. And to achive this we will start by extracting data from Kaggle, then we will do some data cleaning on this data and after we will load this data into a postgresql by creating a database and making sure everything is fine. And the final part will be related to maving the cleaned to a file on our local machine connected to our github repository
### Description of the used data
The data used in this project eas obtained from [Kaggle](https://www.kaggle.com/datasets/azminetoushikwasi/lionel-messi-vs-cristiano-ronaldo-club-goals?select=data.csv). And it is made of three CSV files. the file containing data of Ronaldo, messi and both Ronaldo and Messi respectivelly. Each file is made of 13 columns described as follows\
1. season
2. competition
3. matchday
4. datasets5
5. venue
6. club
7. opponent
8. result
9. playing_postion
10. minute
11. At_score
12. Type
13. Gial_assist


### General Project Overview
Our project involved creation a dag in python scheduled daily , with diffrent specific tasks being part our of pipeline
#### Extracting and cleaning the data task
In this part we just got the two CSV files available on our local dirctory containing data for Ronaldo and Messi and cleaned them. And the cleaning process was basically related to dealing with null values as well as  organising some values present in spqcific columns to make sure consistency is maintained and to allow a proper analysis.
#### Creating the database in postgresql with the tables and well as values insertion tasks
Here we used the famous python library called psycopg2, which allows us to interect with our postgresql in python. So for this a database called ronaldo-messi was created with two tables named ronaldo and messi and values where inserted  into them from the cleaded csv files.
#### moving the cleaned todataset with the python code into our git folder task
Here we just moved the above three files from the working dirctory into a another file connected to our git hub

\
All the detailed code and explanation can be found [here](https://github.com/JulienAganze/Ronaldo_Messi_Project/blob/master/cr7_messi.py)

