# Gateway Signup App Project Backlog

## Iteration 1
**Normal client: check courses it takes**\
For the server, build an API in Java using SparkJava framework.\
For the persistence, use Hadoop database.
Set up users table.\
Set up a table to store one course data (course staff, students, students' scores), which are copied from JHU course system.\
For the client, use HTML, CSS, and JavaScript.
Set up signup user interface with JHU credentials. Only JHU staff and students can signup to application.\
sign up a normal client. Once a client sign up, it creates an account and its data(courses title and Identity: Instructor/Course Assistant/Student) are stored in users table.
This Client can view all its user data in GUI.


## Iteration 2
**Special client: set up retake sessions list**\
Set up table of SP (remark clients who can set up sessions list, initialize with only instructor).
If one client is the instructor of a course, it has special permission to set up sessions list for this course. It is added to SP automatically.\
Instructors of a course can authorize such special permission to other clients if these clients are the Course Assistants of this course. Then these clients are added to SP by the instructor.\
All clients in SP are authorized to set up sessions list (times and durations, maximum number of students, proctors).\
To make it easy for the user to select a date and time period, a calendar will be provided, where users can check directly.\
SP Clients set the threshold of one course and due.
The server generates a link for students to sign up after sessions list have been set up.
Students whose scores are lower than threshold will receive email contain signup link.\
In one course, all instructor and course assistant clients can view the list of proctors in each session.
Students clients can only view the list of each session.

## Iteration 3
**Student client: select a session**\
When students sign up through the link, they will create an account.\
In student clients, students can select a seat in sessions list. Each client can select merely one seat.
Students can reschedule the retake by select a new session.\
All student clients' action are permitted before due.\
In one course, all instructor and course assistant clients can view the list of proctors and in each session and students signed up for each session.
Students clients can only view the list of each session which is not at full strength.\
If one Student's score is higher than threshold, he/she will not be allowed to select a session.

## Iteration 4
**Alpha release: multiple courses**\
We want to add more courses to this application.\
When a faculty member sign up, he/she will view all courses he/she instruct. He/She can select one course to set up sessions list.\
When a student sign up, he/she will view two course lists. One is a list working as a course assistant, and another is a list taking as a student.
When click into course in course assistant list, this account would be a course assistant clients; when select in student list, this account would show sessions of one course.\
The proctors for each session in alpha version is specified by the authorized Course Staff.

## Iteration 5
**Beta release: proctors assignment**\
In this iteration, we need to add the function in Nice-to-have. 
Delete the function of authorized Course Staff assigning Course Assistants as proctors to different sessions. 
Add a Course Assistant subclass to Course Staff. 
Course Assistant Clients can sign up as proctors if number of proctors in one session does not meet the required number. 
Course Assistant Clients can sign up as proctor in multiple sessions with no conflicting times.
