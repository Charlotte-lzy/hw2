# Gateway Signup App Software Requirement Specification

## Problem Statement
Gateway Computing course needs a signup system for instructors and course assistants to set up assessments retaking sessions, and for students to select a suitable session.
With this system (let's call it Gateway Signup), course staff may avoid paying for a premium account in signupgenius.com(in-use system) and customize it to meet course staff' needs.


## Potential Clients
Students in Gateway Computing who need to retake assessments because their scores are under thresholds.\
Course staff who set up retake sessions and act as proctors.


## Proposed Solution
Authorized course staff may set up multiple retake sessions. 
Students who want to retake assessments can select one of the permitted sessions. 
Course Assistants can sign up as proctors in these sessions


## Functional Requirements 

**Must-have**\
As a JHU course staff, I want to signup to Gateway Signup by JHU credentials.\
As an authorized course staff, I want to set up several retake sessions in one week, set the number of proctors, the number of maximum number of students, and duration of session.\
As an authorized course staff, I want to the system can recommend some suitable time according to students' time zoom, so that all students will find suitable time.\ 
As an authorized course staff, I want to create the threshold and send a retake signup link to students whose scores are under the threshold by JHU email, so that only such students would signup for retakes.\
As a course staff, I want to view the summary report which includes a lists of the students signed up for each session.\
As a JHU student, I want to signup to Gateway Signup by signup link from course staff using JHU credentials.\
As a students, I want to view all available sessions marked with number of spare seats so that I would find out which session suit me most.\
As a students, I want to signup only one session so that I would retake assessment only once.\
As a students, I couldn't view the list of students and proctors signup for each session.


**Nice-to-have**\
As a Course Assistant, I want to view all sessions whose number of proctors less than required number, so that one session won't have too many proctors.\
As a Course Assistant, I want to signup as proctor in sessions


## Software Architecture & Technology Stack
Gateway Signup Application is a Web application, conforming to the Client-Server software architecture.\
For the server, build an API in Java using SparkJava framework.\
For the persistence, use Hadoop database.\
For the client, use HTML, CSS, and JavaScript.
