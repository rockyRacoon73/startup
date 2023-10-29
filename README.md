# MovieLog

# Description Deliverable

### Elevator Pitch
Would you like to share your enthusiasm for a particular movie with your friends? Want to know what people are saying about the latest blockbuster? The MovieLog application allows you to read and publish reviews so you can hear opinions on the latest films. 

### Design

**sign in page** 
![image](https://github.com/rockyRacoon73/startup/assets/90075184/ec95815e-35ef-4b5e-b92a-ef6aaecd88f4)



**Reviews Page**
![Reviews Page](https://github.com/rockyRacoon73/startup/assets/90075184/d3f835c8-8d0e-4d5b-ac5f-466474f3a4f3)

**User Profile**
![user page](https://github.com/rockyRacoon73/startup/assets/90075184/9c78d783-5cb8-496e-9d83-7776ce02e8dc)


**Individual Review Page**


![individual review](https://github.com/rockyRacoon73/startup/assets/90075184/8a0f4fa3-84b6-4063-b587-1b0576db7269)


**Publish Review** 


![image](https://github.com/rockyRacoon73/startup/assets/90075184/dd8c925b-ed41-4049-a26e-627ec5472b55)






### Key Features
* Publish your own movie review
* View a page filled with hot reviews
* read full reviews
* ability to like a review
* abilty to view a user's profile containg all their reviews


  

### Technologies
* Authentication: User login page. Current users name is displayed in top right corner of each page.
* Database data: Stores users - has profile and lists of published reviews as well as user entry lists for saved profiles, media.
* WebSocket data: updates number of likes on reviews and avg ratings on media pages


# HTML deliverable
Built structure for application using HTML

Reduced the complexity of the project and altered Description deliverable.  

## HTML pages
index.html - log in/ sign up page 
reviews.html - view titles of published reviews, ranked by most likes
profile.html - view the profile and reviews of a particular user
fullReview.html - read the full review 
publish.html - form for publishing a review 

## Links 
* header menu links to log in page, reviews.html, and publish.html
* any username links to that user's profile
* any review title links to  fullReview.html

## Text
* each review is represented by a text description
  
## images
 included image on the log in page and reviews page

## login
input boxes for username and password (character limited) and login or sign up buttons

## Database 
review data is pulled from database

## webSocket 
review like count represents realtime likes

## 3rd party API
added space on reviews.html for movie quotes to be added through 3rd party service




