This repo is a clone of 
https://github.com/nelaturuk/education_pathways.  


# Activity 1

![](Screenshots/activity_1.png)

# Activities 2-5

Home Page
![image](https://user-images.githubusercontent.com/22103819/198145031-fd8a06bc-60f6-4c70-8035-f225b41824c4.png)

Results Page - Form
![image](https://user-images.githubusercontent.com/22103819/198149734-b35fa762-1d82-4b12-b0e3-8ead7b7a81af.png)

Results Page - Results Table
![image](https://user-images.githubusercontent.com/22103819/198149805-ca838c86-3522-477f-80f5-bafa0e6192bf.png)

# Activity 6  
User Stories:  
![image](https://user-images.githubusercontent.com/68239498/198129751-a61c153c-0907-4faf-948f-dc637aabe9ec.png)  
![image](https://user-images.githubusercontent.com/22103819/198131707-05b82c1d-6aad-4463-b5ab-4b0ffde3effe.png)

Prototypes:  
![image](https://user-images.githubusercontent.com/68239498/198129813-9af3c342-3fc3-44dd-b0ad-0517d926f55c.png)  
![image](https://user-images.githubusercontent.com/68239498/198129969-85cc9c0f-c870-40d1-99f2-20d9db884c3d.png)
![image](https://user-images.githubusercontent.com/22103819/198131907-ad846635-6974-49df-9b7d-d372ded69ed9.png)





# CARTE Education Pathways

## Description
Welcome to CARTE's in-development tool for course selection at UofT. Education Pathways allows for more intelligent course searching, by matching not just the terms you search, but ones relevant to them. The more terms you search for, the more relevant your results will be! Even try searching across disciplines for the courses that best cover each.

Whatever year you are looking for, Education Pathways will also suggest courses in earlier years that will best help you to prepare. To get the most out of this, try searching for courses in a later year and see what is suggested for your current one.

We are looking for feedback to improve Education Pathways and make it more useful for students. If you have ideas or suggestions, please email us!

## Setup Instructions

### With Docker



## Repository files:

`./Procfile ./wsgi.py` *tells gunicorn how to run the program*

`./environment.yml  ./requirements.txt` *specifies python requirements for anaconda and pip respectively*

`./__init__.py` *main flask code*

`./readme.md` *this file*

`./resources:` *contains datasets used in the program*

`course_vectorizer.pickle df_processed.pickle`

`course_vectors.npz       graph.pickle`

`./static:` *contains any static elements of the webpage, in this case just the CARTE logo*
`CARTE_logo.jpg`

`./templates:` *contains flask templates for rendering HTML*

`_formhelpers.html course.html       index.html        results.html`
