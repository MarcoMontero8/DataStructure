# DataStructure
Students are asked to implement an O.O. C++ program to simulate the process of Final Degree Projects to students of Computer Science.
To do so, the program will read CSV files with the following data:
1.	List of available projects. With number (int), name (max. 50 chars) and project description (max. 200 chars).
2.	List of students waiting for assignment. With id (name and surname, like in UAH mail without @) (max. 50 chars), average mark in all degree courses, and list of requested projects (up to 10) by number.

For the assignment of projects to students the program will do the following steps:
1.	Creation of an stack with the projects from the list (not deleting them). The stack will have the project with the lowest number in the top of the stack.
2.	Extraction of every project from the stack. 
1.	For a project extracted the program will search in the list of students ordered by mark, for the first student that requested the project, and remove its record from the list.
2.	With the project id and the student id, a new record is created and stored in a queue.
3.	Every pair of project-student is extracted from the queue. The project id is used for recovering the info of the project from its list, and the student id is used for recovering its information from the list ordered by id. A line with all the information for every assignment is printed in the screen.
