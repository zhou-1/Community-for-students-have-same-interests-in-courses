# Community for students have same interests in courses   
Get recommanded courses based on your own choices and our algorithm, communicate and make friends in our accademic web community.    
Deploy a django app through azure. (future)       
https://stories.mlh.io/deploying-a-basic-django-app-using-azure-app-services-71ec3b21db08    

## Final Set up for the project      
### Needed files and programs       
All files needed in [FinalFiles folder](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/tree/master/FinalFiles)    
Download the zipped file inside the folder.   
    
OR     

Use ``` git clone https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/tree/master/FinalFiles ```    

### Manual for setting up        
Operating system need: Linux     
Programming language: Python     
  
First, please download it and unzipp it in Linux environment.   
Second, download python3 and install.   
Third, download Django and install.    
Forth, go to the folder, use command ```manage.py runserver 0.0.0.0:8080``` to run the server, 8080 will be the port we use on webpage.   
Fifth, go to the browser to check the webpage, http://192.168.0.1:8080. It will show community webpage first, then quora questionaire page and lastly results from our recommendation algorithm.          

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
Finished sprint 3.     
Working on final wrap-up.    

<hr> 

## Sprint 1
First, sprint 1 introduces product definition including product mission, target users, user stories, MVP and user interface.    
Second, sprint1 also lists the product survey about comparing with other similar products.    
Third, sprint 1 shows system design about Major Components, web framework, a little bit about goal of algotithm.      
Detailed sprint 1 materials and processes are in sprint 1 folder.    

## Sprint 2  
In sprint 2, we focused most on web development; also we talked a lot about algorithm and leave for sprint 3 to decide the most proper algorithm.      
For first of the main webpages, questionaire, it is used for new user to select the academic areas for courses recommendation use in the future, also is used for existed users to update their academic interests before the new semester so they can get new recommendations for courses for every semester.      
For second of the main webpages, user register/log in system, it is used for new user to register for our system; also registered user can post their thoughts in community and share their ideas under others' comments.It can be generaly seperated as User / Blog / Media Directories.
The Blog Directory contains the templates of the main pages, in which there are base, about and home page.
The User Directory contains most user-related pages like login & logout page, registerpage and profile pages.
The Media Direcyoru contains all the media files like profile pictures / defult pictures for each user.
The whole program can achieve the following fuctions:
Register system for new users, SQLlite for saving the user datas.
Basic wrong message if the username or password is incorrect or unsecure.
After login there will be a profile button and quora button for users to edit their own profile (including name, email, pictures, etc.) and can jump to the questionare by clicking the quora button.
The user can logout and will not be able to see the profile and quora button again. But still can see the home button and about button.
The home button and the name "CourseFront" button can let the user go back to the home page.
(If you regard this community as a boundless ocean these button can bring you home no matter where you are.)
The about button can introduce the web to all the visitors to this website even to those who haven't registered.
In the home page everyone can see the blogs that are posted. Including the author, time, title and content.
The administrator can add other administrators and manage the blogs, like editing all the informations above.
     

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
The home page looks like below:
![p1](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p1.png)
The user can click the 'CoursFront' or 'Home' button to go back home.
by clicking the 'About' button the user can go to the About page, which contains the basic informations about this web.
The about page looks like below:
![p2](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p2.png)
You can click 'Login' button to login to the web. If you are new user you can click 'Register' Button to register.
The login page looks like below:
![p3](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p3.png)
A good thing is if you are not a registered user but still clicked the 'Login' Button, there is still a link of register page
to help you go to the register page.
The register page looks like below:
![p4](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p4.png)
Once you have successfully registered there is a link to help you go back to login the page looks like below:
![p5](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p5.png)
After you login there will be a little difference on the upper right corner.
'Quora' Button is a questionare. 'Profile' Button is your personal profile. 'Logout' button can help you logout.
The loggined home page looks like below:
![p6](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p6.png)
The profile page contains a user picture and email and username.
The page looks like below:
![p7](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p7.png)
The 'Quora' button can help you jump to the questionare page.
After clicked the logout file you will be back to the original home page.
## Sprint 3   
In sprint 3, we did a lot on 3 parts: user login/register system, questionaire web system and recommendation system.    
For user login/register system, we updated several links to different web pages.       

For questionaire web system, we added several academic questions for better course recommendation, also for each question, there will be different response on it; at the end of user finishing questions, the system will show a webpage for loading, at the meantime, our algorithm will match best course for user based on his/her choices, when the algorithm finishs its process, our page will show the result and have a link for user to community. Right now, the user interface, loading page is basic. In the future, we will modify it to be better. Also, we will add function to show the result after loading page, we will record the answer to a text file which will be used as input for the algorithm.     
Demo for more academic questions:    
![demo question image](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/1.PNG)     

For the recommendation system, we utilize the k-nearest neighbors algorithm to classify users into different predefined groups based on their answers of the quetionnaire. In the questionaire, we add 10 questions to evaluate each user, the first one is to ask whether the user is undergrad or grad student, and the other nine are to acquire the the grades of some pre-requisites courses of three specialized academic areas, which are robotics, data analytics and cybersecurity. For the first question, we evaluate with point 0 and 2 each for undergrad and grad. For the rest nine, we rate users' performance from 3 to 0, each for A+/A, B+/B, lower/haven't taken yet. Now we have got a 10-element vector to assess our users. On the other side, we create a sample set written in txt file to train our KNN network, and classify them into nine group, which are 'A1':'Robotics Entry Level', 'A2':'Robotics Medium Level', 'A3':'Robotics High Level, 'B1':'Data Analytics Entry Level', 'B2':'Data Analytics Medium Level', 'B3':'Data Analytics High Level', 'C1':'Cybersecurity Entry Level', 'C2':'Cybersecurity Medium Level', 'C3':'Cybersecurity High Level'. Once the user finish the questionaire part, their answer will generate a coresponding user.txt file. Then the trained KNN network will calculate their label, and classify them into the group.


### sprint 3 set up     
There are three set up manual for sprint 3.      
#### Manual for questionaire web system              
Operating system need: Linux    
Programming language: Python   

In sprint 3, there is a [zipped file called matchApp.zip](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/Sprint3/matchApp.zip).    
First, please download it and unzip it in Linux environment.   
Second, download python3 and install.   
Third, download Django and install.    
Forth, go to the folder, use command ```manage.py runserver 0.0.0.0:8080``` to run the server, 8080 will be the port we use on webpage.   
Fifth, go to the browser to check the webpage, http://192.168.0.1:8080.      
Sixth, choose the result based on your background and submit your answer.

Below is the final setted up demo image.    
![Image description1](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/sprint3_into.png)
![Image description2](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/sprint3_question.png)


#### Manual for user register/login system      
In sprint 3 we finished the administrator system.
by going to the ulr/admin you can go to the administrator page, which looks like below:
![p11](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p11.png)
It requires an admin account like a super user. For example, the admin id is Osama, password is osama123
then you can junmp to the page like this:
![p12](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/img/p12.png)
#### Manual for algorithm    
Operating system need: Linux / Windows
Programming language: Python   

In sprint 3, there is a [zipped file called KNN.zip](https://github.com/zhou-1/Community-for-students-have-same-interests-in-courses/blob/master/Sprint3/KNN.zip).    
First, please download it and unzip it in the required environment.    
Second, download python3 and install.    
Third, run the KNNmactch.py file in the terminal with ```python KNNmatch.py```    
Forth, go to the folder, use command ```manage.py runserver 0.0.0.0:8080``` to run the server, 8080 will be the port we use on webpage.    
Fifth, open the browser to check the classification result.    


