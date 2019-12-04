# Community for students have same interests in courses   
Get recommanded courses based on your own choices and our algorithm, communicate and make friends in our accademic web community.    

## Final Set up for the project      
### Needed files and programs       


### Manual for setting up        


### User example
We have bunch of users, like one of them, Z, want to find proper course in Electrical and Computer Engineering major in Boston University. Z can use our web questionaire system (including our recommendation algorithm) to get recommended courses from us; moreover, he can also go to our course community to check others' sharing and review.     
We also have bunch of users, like one of them, A, want to find classmates or even friends in same interesting coourse. So in our community, if they find they have same interests in course, they can add each other as friend (leave email, social media to add friend in post). In the future, we will add private chat in our community system, so users can chat through our community system instead of adding social media friends which protect their privacy if they want.    
In the future, we will also open our algorithm as open API for people who are interested in matching and recommendation algorithm.      

### Architecture    
Below is the architectur image for our project.    
![Image description](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/architecture.JPG)   
    
    
## Process
Finished sprint 1.      
Finished sprint 2.  
Working on sprint3, almost done.     
Preparing for final wrap-up.    

## Sprint 1
First, sprint 1 introduces product definition including product mission, target users, user stories, MVP and user interface.    
Second, sprint1 also lists the product survey about comparing with other similar products.    
Third, sprint 1 shows system design about Major Components, web framework, a little bit about goal of algotithm.      
Detailed sprint 1 materials and processes are in sprint 1 folder.    

## Sprint 2  
In sprint 2, we focused most on web development; also we talked a lot about algorithm and leave for sprint 3 to decide the most proper algorithm.      
For first of the main webpages, questionaire, it is used for new user to select the academic areas for courses recommendation use in the future, also is used for existed users to update their academic interests before the new semester so they can get new recommendations for courses for every semester.      
For second of the main webpages, user register/log in system, it is used for new user to register for our system; also registered user can post their thoughts in community and share their ideas under others' comments.     

### sprint 2 set up     
There are two set up manual for sprint 2.    
#### Manual for questionaire webpage    
Operating system need: Linux    
Programming language: Python   

In sprint 2, there is a [zipped file called matchComm2.zip](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/Sprint2/matchComm2.zip).    
First, please download it and unzipp it in Linux environment.   
Second, download python3 and install.   
Third, download Django and install.    
Forth, go to the folder, use command ```manage.py runserver 0.0.0.0:8080``` to run the server, 8080 will be the port we use on webpage.   
Fifth, go to the browser to check the webpage, http://192.168.0.1:8080.      

Below is the final setted up demo image.    
![Image description](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/Sprint2/IndexView.PNG)

#### Manual for user register/login system    




## Sprint 3   
In sprint 3, we did a lot on 3 parts: user login/register system, questionaire web system and recommendation system.    
For user login/register system, we updated several links to different web pages.       

For questionaire web system, we added several academic questions for better course recommendation, also for each question, there will be different response on it; at the end of user finishing questions, the system will show a webpage for loading, at the meantime, our algorithm will match best course for user based on his/her choices, when the algorithm finishs its process, our page will show the result and have a link for user to community. Right now, the user interface, loading page is basic. In the future, we will modify it to be better. Also, we will add function to show the result after loading page, we will record the answer to a text file which will be used as input for the algorithm.     
Demo for more academic questions:    
![demo question image](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/1.PNG)     

For the recommendation system, we utilize the k-nearest neighbors algorithm to classify users into different predefined groups based on their answers of the quetionnaire. In the questionaire, we add 10 questions to evaluate each user, the first one is to ask whether the user is undergrad or grad


### sprint 3 set up     
There are three set up manual for sprint 3.      
#### Manual for questionaire web system              
Operating system need: Linux    
Programming language: Python   

In sprint 3, there is a [zipped file called matchApp.zip](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/Sprint3/matchApp.zip).    
First, please download it and unzipp it in Linux environment.   
Second, download python3 and install.   
Third, download Django and install.    
Forth, go to the folder, use command ```manage.py runserver 0.0.0.0:8080``` to run the server, 8080 will be the port we use on webpage.   
Fifth, go to the browser to check the webpage, http://192.168.0.1:8080.      
Sixth, choose the result based on your background and submit your answer.

Below is the final setted up demo image.    
![Image description1](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/sprint3_into.png)      
![Image description2](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/sprint3_question.png)        


#### Manual for user register/login system      

       
#### Manual for algorithm (.py file)      


 
