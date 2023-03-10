# Vedant Prajapati

This Repo is a clone of https://github.com/ECE444-2022Fall/Assignment_1_starter_template

# Education_Pathways

This is a modified version of the previous Assignment1 template.

The deploye version can be found at https://lab3-docker.herokuapp.com.


# Activity 2

![](images/activity_2.png)

# Activity 3

![](images/activity_3.png)

# Activity 3

![](images/activity_4_1.png)

![](images/activity_4_2.png)

![](images/activity_4_3.png)


## Changes
+ Removed hardcodes of backend urls.
+ Removed hardcodes of database, and replace the database with dummy static data.


## How to run it locally

+ Enter the repo directory
+ Create a virtual environment if you haven't done this before. Activate it. 
```powershell
# Windows
py -3 -m venv venv
venv\Scripts\activate

# For Mac and Linux, please check the link: https://flask.palletsprojects.com/en/2.2.x/installation/
```
+ Install dependencies (if you haven't done this before).
```powershell
pip install -r requirements.txt
```
+ Enter the `Education_Pathways/` directory, run the backend
```powershell
flask --app index --debug run
```
+ Enter the `Education_Pathways/frontend/` directory
+ Make sure the `baseURL` is set as `localhost:5000`
```javascript
# Education_Pathways/frontend/src/api.js
export default axios.create({
   baseURL: "http://localhost:5000/"
});
```
+ Make sure the proxy link in package.json is set as "http://localhost:5000/"
```json
// Part of Education_Pathways\frontend\package.json
"private": true,
"proxy": "http://localhost:5000/",
```

+ Build and run the frontend:
```powershell
npm run build
npm start
```
+ Then you will see the application at `localhost:3000`


## Build and run with Docker

For detailed instructions on Docker, please refer to the documents for Lab3 on Quercus.

+ Change the proxy link in package. Remember to change it back to "http://localhost:5000/"
```json
// Part of Education_Pathways/frontend/package.json
"private": true,
"proxy": "http://host.docker.internal:5000/",
```

```powershell
# Under the root directory
docker compose up --build
```
