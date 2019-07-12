# simple-heroku-flask-app
Set up a simple web app within minutes. The app is hosted on Heroku and the backend is written in python using Flask.

## Requirements
Make sure you have the following installed:
* Git
* [Heroku Cli](https://devcenter.heroku.com/articles/heroku-cli)
* Python (version 3.6.8) 

## Clone this template
```
git clone https://github.com/xRadne/simple-heroku-flask-app.git
cd simple-heroku-flask-app
```

You should now be able to run the app on your machine:
```
python flask_app/flask_app.py
```

## Create the heroku app
Now go ahead and create a new app. 

Make sure you are logged in to heroku with the command `heroku login`.

Note that your apps name (`[your-app-name]`) needs to be unique. You can omit this parameter to get a random name automaically assigned.  
```
heroku create [your-app-name]
```
Once your app has been created you can push the code to heroku using the following:
```
git push heroku master
```

Now go to [https://[your-app-name].herokuapp.com/]() to see your app.

## Updating your code
You can update your code at any time by pushing your commits to heroku. Make sure you are on the correct remote. 
```
heroku git:remote -a [your-app-name]
git push heroku master
```