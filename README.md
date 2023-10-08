# HemoWin

EERD:


Read me: 
Setup for jar:
– Make sure the jar and the config.properties file are in the same directory.
– edit the properties file with your details 
– you will find three values: url, root and password Update it with your workbench fields.
– Once you are done with it, load the dump file in your workbench and check whether the db has been added.
– now run the jar using java -jar {jar-name}
– the application will open up with three buttons to go to three pages respectively 
Setup for project using intellij:
Open the project in intellij run maven clean install to load all the dependencies.
Update the values in config.properties file for your workbench. The file is in the resources folder.
Run the Application.class the Java swing app will pop up.


—----------Interactions—----------
First :Donor Login Page 


You will be asked to enter your username and password.
If you keep any one of them empty the application will tell you.
It will not let you in until and unless you provide the username and password that are present in the DB.
Once you provide the right details it will take you to the Donor homepage.


Second : Registration page
This page will have a form to register a new donor.
The application is highly advanced in handling wrong inputs by the user and won't let you proceed if you miss any of the required input fields.
If the username is not unique then the application will give you the popup to try some other username.
If you put all the details correctly then you will be sent to your new donor  home page.
Third: Worker login page
There is not registration for worker, we will be registering them from back end and providing them ids.
Some of the ids you can use to test : 
username :worker1, password: password1
Username :worker2, password2
Or you can run select * from the worker to find out these details to test.
Once you provide the correct details you will be logged into the Worker Home page.


Donor Home Page:
In this page you will be seeing active contests and the option to register for them.
Click on the register button and the contest will move to the registered contest and the option to book an appointment will pop up.
If you click on the book appointment button the form will open up to fill appointment details:


Form :Now to book an appointment you will have to select the worker to whom you want to meet for the donation using the drop down menu. 
You have to select the date on which you want to donate plus select the contest in which you will be donating. Here you will only see ongoing registered contests by you in the drop down menu.
After booking an appointment you will be back to the homepage again.


Back to the home page.
You will see the upcoming appointment with an option to delete them.
On top of the page you will see user details and an option to change password.
Once you click on the button a form will popup for the new value.
There is also a global leaderboard which will be visible to all the users and be updated at realtime. The leaderboard displays the top donor of every contest.


Worker home Page:
Worker will see any active appointment under his name and can accept them.
Once he clicks on the accept button the page will open up for the blood donation quantity for the user once the worker inputs and submits it he will be back to the worker homepage again. The active appointments will be updated in real time.
This page also provides workers the option to change passwords with similar flow as donors.



Lessons Learned:

Technical Expertise Gained:
Throughout this project, we gained a deeper understanding of relational database management systems (DBMS) and how to work with them effectively. Specifically, we became more proficient in using MySQL to store, retrieve, and manipulate data related to blood donations and contests. We also learned how to build RESTful web services using Java 11 and the Spring Boot framework. Additionally, we gained experience with Java Swing and the JFrame component, which allowed us to build a user interface that is both dynamic and user-friendly.

Insights:
We learned the importance of data integrity and consistency when working with a DBMS. By setting up proper constraints and relationships between tables, we were able to prevent data inconsistencies and ensure that our application operated as expected. Additionally, we gained valuable insights into user interface design, such as the importance of minimizing user input and providing clear feedback.

Alternative Designs/Approaches:
During the course of this project, we considered various alternative designs and approaches for our user interface. For example, we contemplated using a web-based front-end framework, such as React or Angular, instead of Java Swing. However, we ultimately decided to use Java Swing due to its ease of use and familiarity with the Java programming language. Additionally, we considered using a different layout manager, such as GridBagLayout, to improve the layout and alignment of our components.

Non-Functioning Code:
While we encountered some issues with our Java code and user interface during development, such as NullPointerExceptions and layout issues, we were able to resolve them through collaboration and debugging. We also gained experience with development tools such as IntelliJ IDEA and MySQL Workbench, which helped us to streamline our workflow and improve our productivity. We made sure to document any issues and their resolutions in our version control system, Git, to ensure that our code and user interface were always up to date.

Future work:

Planned Uses of the Database:
In the future, we plan to utilize the database for additional features such as worker signup, worker contest creation, and donation history tracking. By allowing workers to sign up and create contests, we can incentivize them to promote blood donation at their facility and help increase donations. Additionally, we can implement an automated system for reward allocation based on the amount and frequency of blood donations made by users. Finally, we plan to create a donation history page where users can track their past donations and the rewards they received, as well as view their progress towards meeting donation milestones.

Potential Areas for Added Functionality:
Some potential areas for added functionality include the ability for users to search for nearby donation facilities and schedule appointments directly through the application. This would not only provide added convenience for users, but also help increase donations by making it easier to find and schedule appointments at nearby facilities. Additionally, we could implement a feature where users can invite friends and family to join the application, and earn bonus rewards for each new user they refer. Finally, we could explore the possibility of integrating with social media platforms to further promote blood donation and incentivize users to share their donations with their network.


