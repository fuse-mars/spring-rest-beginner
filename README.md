# spring-rest-beginner
Beginner guide to creating rest api using spring boot

## Goal
Create a system that tells you the time in one city, if you give it(the system) another time from a different city.

```sh
# what time is "10:30 PM kathmandu", in New York?

# input
curl http://localhost:8080/api/v1/time/New York?time=10:30 PM&city=Kathmandu

# output
{
  "city": "New York",
  "time": "12:45 PM"
}
```

## Step by Step

* Prerequisite: You should have your app running locally!

* Initialize git repository in your project

```sh
# inside the root folder of your project
git init
```

* Create a `develop` branch
```sh
git checkout -b develop
```

* Create an empty **Github repository**
  * Go to [Github](https://github.com)
  * Look for *New repository* button, then click it
  * Enter the name `time-checker` of your repository
  * Click *Create repository*
  
* Configure your local machine to send code to Github server
```sh
git remote add origin <url of the repository you created in porevious step>
```

* Add and push all your source code to github
```sh
git add .
git commit -m "create one api that allows users to view time from different cities"
git push origin develop:develop
```

* Configure **Travis-ci** to run your tests

TODO








