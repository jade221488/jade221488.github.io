---
layout: default
title: "Hailey's CS499 EPortfolio"
---

## **Welcome to my Computer Science Capstone ePortfolio!**

My name is Hailey Bondra. I majored in Computer Science graduate from Southern New Hampshire University. Within this site, there is a self-assessment reflecting on my academic journey, a video code review, and three technical artifact enhancements. My growth is highlighted across two projects showcasing three core areas of software development: Software Design and Engineering, Algorithms and Data Structures, and Databases.

---

## **Self Assessment**

Building this ePortfolio has transformed my mindset, shifting my perspective from a student into an analytical software developer who can solve real-world problems. I have taken abstract concepts and applied them to demonstrate my skills through three enhancements from my previous work. Throughout my time in the computer science program, emerging trends such as AI and machine learning have shifted my learning. Expanding my knowledge in how to work with these newer systems is beneficial. However, understanding foundational programming practices is an important skillset I am most proud of. 
  
A skill I have continuously refined throughout this program is being able to work well in collaboration with others to develop software. This includes learning how to effectively communicate with peers in managing workloads, organizing deadlines, and ensuring we all remain cohesive throughout the project. Furthermore, I have learned more about client-facing communication and learning how to bridge the gap between software development and meeting business requirements.
  
The first artifact to be enhanced is a buffer overflow module that can detect and handle when there is a buffer overflow occurrence. The enhancement plan was to transform the program to be a reuseable and secure input processor that can handle buffer overflow, input validation, and sanitization. 
  
Software design and engineering skills are demonstrated in this enhancement by implementing memory safety, input validation, sanitization, safe error handling, defensive programming, and problem solving. Memory safety ensures that the program can identify and handle any input that exceeds bounds. Input validation checks the user’s input to ensure that there is no malicious data, if there is then the program will block any harmful data from entering. Input sanitization modifies any unwanted input. Safe error handling protects the program from crashing and provides generic error messages that do not leak sensitive data. Defensive programming practices anticipate unexpected inputs or program failures, this mindset helped me develop code that mitigates these occurrences from happening.
  
The second artifact is a weight tracking mobile application where the user can create an account to track their daily weight and progress over time. The log in screen allows the user to create an account, log in, and recover their password if needed. There is one database table that assists the log in screen as it holds the user’s account information such as username and password. The main screen displays the user’s weight goal along with their current progress. There are two database tables for the main screen where one holds the user’s daily weights with the corresponding date it was logged and the second database table holds the user’s goal weight. Lastly, a weight history screen will display all logs from the database that stores the user’s weight history. This artifact had two enhancement plans: implement a prediction algorithm that will display an estimated amount of time it will take the user to reach their goal from their current weight; this will be displayed on the main screen. The second enhancement plan improves how information is stored in the database. Previously, when information was stored by a user the information was not linked to the user that entered it in the system this made the application non-multi-user friendly. To solve this issue a unique user ID will be attached to each user account created as well as all information entered or updated in the database.
  
Data structures and algorithms skills are demonstrated in this enhancement through algorithm design, time complexity, and problem solving. Algorithm design skills are shown from the prediction algorithm that uses the user’s weight history and goal weight to estimate the time it will take the user to reach their goal weight. Time complexity is considered here as the algorithm will process the weight history using a single traversal with a time complexity of O(n)  where n is the number of weight logs. Database skills are demonstrated through database design, SQL proficiency, database management, and problem solving. Database design skills are demonstrated from the improvement of the current database as the data stored is now connected the user entering the data. SQL proficiency is shown using a primary key to generate a unique ID number and a foreign key that links the user’s account with the stored data together. Database management skills are shown as the data stored is better structured to handle multiple users as the application continues to grow.

---

## **Code Review**

[Click Here for Code Review Youtube Video](https://youtu.be/EOS6yrbGW5o)

---

## **Enhancement One: Software Design and Engineering**
### Enhanced Artifact: Secure Input Processor
#### **Repository Link**

- [Click Here for Enhancement One Repository](https://github.com/jade221488/jade221488.github.io/blob/main/CS499_SoftwareDesignEngineering.zip)

The artifact originally identifies and demonstrates a buffer overflow vulnerability. The program initializes and declares a set input size that limits how much input it can hold. The program then prompts the user for an input. It checks if the user’s input is more characters than what can be held. If the user’s input is too long, then a message will display prompting the user of a buffer overflow error and throws away the remaining characters from the user input that cannot be held and stops the program. If the user’s input fits the parameters of the set input size, then the program will output the user’s input along with the account number. The original artifact came from the course CS405 Secure Coding and was created in April of 2026. 
	
I selected this artifact to include in my e-portfolio as the program is simple, yet it had the potential to grow into a modular and secure program. The artifact was improved by creating three reusable functions: a buffer overflow check, sanitization, and validation. I had created a function for the buffer overflow check to help better structure the program into a reusable module. The sanitization function cleans and modifies any unwanted input such as whitespace characters. The validation function prevents malicious data from entering the program, only alphanumeric characters can enter the program. I had cleaned up the documentation of the code so that if another developer to look at the artifact it is easily understood. This artifact now demonstrates secure software development skills such as memory safety, input validation, sanitization, safe error handling, defensive programming, and problem-solving skills.  
	
I did meet the course outcomes with this artifact as I was able to design and evaluate a solution that followed computer science practices and standards, demonstrate my techniques and skills along with my knowledge of tools, and create a secure artifact that meets secure coding standards. During the process of enhancing the artifact, I thought the artifact I had chosen may have been too small of a program to demonstrate all the skills and abilities I learned throughout my degree. However, I found that an artifact that is simple can be meaningful if it has quality to it. 

---

## **Enhancement Two: Data Structures and Algorithms**
### Enhanced Artifact: Weight Tracker Mobile Application

The artifact is a mobile web application that is a daily weight tracker where the user can create an account, log in, and recover their password. The main screen once logged in displays the user’s weight goal, a progress bar showing how far they are from their goal weight, the estimated time to reach their goal, a prompt for the user to log their daily weight, and a button to navigate to the weight history screen. The weight history screen displays the user’s weight entries they have logged over time. The mobile application was originally from the course CS360 Mobile Architecture and Programming and was created in February of 2026.
	
I selected this application as an artifact for my ePortfolio as I knew the original project was not my best work. The original artifact had most of the structure in place and was a functional application, however it lacked further detail and design to make the application more appealing for users to want to use. In this enhancement I implemented a prediction algorithm that displays an estimate of the time it will take for the user to reach their goal. The prediction algorithm works by first checking if there are at least two weight entries logged to generate an accurate estimate. The system then checks if the goal is already reached, if so, it will display a message to the user that goal is reached. If there are at least two weight entries and the goal has not been reached, then it looks at all the user’s weight entries and corresponding dates they were logged. The algorithm calculates the user’s average rate of weight change over time. With this information, the algorithm creates an estimate of how long it will take the user to achieve their goal weight from their current weight. 
	
Additional to the data structures and algorithms enhancement, I worked on improving the overall application. I changed the design for all three screens and application logo, so it looks more user friendly and cohesive. I removed the SMS Permissions feature completely as it was not functional in the original artifact. The forgot password feature on the log in screen is functional so that users can enter their username and answer a security question to create a new password. Lastly, I updated the database to be able to handle multiple users better this will be further discussed in enhancement three.
	
I met course outcomes three and four in this enhancement as I used algorithmic principles and computer science practices to implement a feature that further enhances the application. I was able to demonstrate the skills and tools I know in computing practices in this enhancement. Throughout this process I was challenged throughout the process as this application is much larger than the first artifact I chose for enhancement one. I do think there are still some improvements in this application I would implement in the future to further ensure the application meets secure coding standards.

---

## **Enhancement Three: Databases**
### Enhanced Artifact: Weight Tracker Mobile Application

The artifact is a mobile web application that is a daily weight tracker where the user can create an account, log in, and recover their password. The main screen once logged in displays the user’s weight goal, a progress bar showing how far they are from their goal weight, the estimated time to reach their goal, a prompt for the user to log their daily weight, and a button to navigate to the weight history screen. The weight history screen displays the user’s weight entries they have logged over time. The mobile application was originally from the course CS360 Mobile Architecture and Programming and was created in February of 2026.
	
This application was selected as an artifact for my ePortfolio as the application needed a lot of improvements. The original application lacked effort as when I originally created it. I felt I could best reflect the skills I have learned during my time in college in this application.
	
The latest enhancement now allows the application to handle and store multiple users’ information in their respective places. In the original application, if a user were to enter a weight entry, then that information would be shared amongst other accounts as there was no link connecting the user’s account to their information that they entered in the system. I implemented a unique user ID that is linked across to all information the user enters into the application. This was done with the use of primary and foreign keys. The primary key acted as the unique user ID for each registered user. The foreign key links all information entered by the user back to the unique user ID. 
	
I met course outcomes three and four in this enhancement as I used algorithmic principles and computer science practices to implement a feature that further enhances the application. I was able to demonstrate the skills and tools I know in computing practices in this enhancement. During this enhancement I learned more in depth about SQLite databases and how to implement foreign keys. A challenge I faced in this enhancement was familiarizing myself with Android Studio and meeting the standards the platform has when developing applications.

---
