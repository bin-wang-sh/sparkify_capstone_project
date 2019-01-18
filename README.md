# Sparkify Capstone Project

## 1. Installation
I use python 3.5 to create this project and the main libraries I used are:
- Flask==1.0.2
- gunicorn==19.9.0
- matplotlib==3.0.2
- numpy==1.15.4
- pandas==0.23.4
- plotly==3.4.2
- scikit-learn==0.20.2

Please check requirement.txt for the detailed packages information.

## 2. Project Motivation

The project  contains a  subset (256MB). I create a spark cluster that consists of one driver and 2 executors as follows:
 ![GUI1](IBM_1.jpg 'Input window')
 on the IBM cloud.  deploys the  your cluster on the IBM cloud. Instructions for setting up your Spark cluster is included in the last lesson of the Extracurricular Spark Course content.

You can follow the steps below to guide your data analysis and model building portion of this project.


For this Udacity project I'm looking at the interactions that users have with articles on the IBM Watson Studio platform. I use several recommendations to shows the articles that are most pertinent to a specific user.
In order to determine which articles to show to each user, I perform a study of the data available on the IBM Watson Studio platform. I use the following recommendations to recommend articles
- Rank based recommendation
- User based collaborative filtering recommendation
- Content based recommendation
- Matrix Factorization recommendation
I build out a content based recommendation system using the NLP skills.  And the above recommendations are used in the different situations and they are combined a whole solution. Finally I move the notebook into a web application, and blend codes into a class that can be easily used with a web application.

## 3. File Descriptions

- Recommandations with IBM\
   - README.md
   - Recommendations_with_IBM.html
   - Recommendations_with_IBM.ipynb
   - project_tests.py
   - user_item_matrix.p
   - data\
     - articles_community.csv
      - user-item-interactions.csv
   - web_app\
     -  Procfile
     -  recommendation
     -  recommendation_app.py
     -  rec_app
     -  requirement.txt
     - data\
       -  articles_community.csv
       -  user-item-interactions.csv
     - recommendation\
       -  cbrecommender.py
       -  data_clean.py
       -  mfrecommender.py
       -  rbrecommender.py
       -  recommendation.py
       -  recommender.py
       -  ucfrecommender.py
    - rec_app\
       -  run.py
       -  __init__.py
       -  templates\
          -  go.html
          -  master.html

## 4.Instructions:

     1. Deploy all files under the web_app directory to web application server.

     2. The web server run the recommendation by the following steps:

         -  The web server inovkes recommendation_app.py via Procfile.
         -  recommendation_app.py invokes rec_app.__init__.py  and listen on 0.0.0.0:3001
         -  rec_app.__init__.py invokes rec_app.run.py to response web request.

     3. The web application address is :

     4. The web page will show as follows:
       - Input Window：
 ![GUI1](IBM_1.jpg 'Input window')


       - Result Window：
![GUI2](IBM_2.jpg 'Result window')




## 5. GitHub link:
   - https://github.com/bin-wang-sh/Recommendation_with_IBM_Webapp

## 6. Licensing, Author, Acknowledgements
This work is licensed under a [Creative Commons  Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/). Please refer to [Udacity Terms of Service](https://www.udacity.com/legal) for further information.
