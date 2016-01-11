# Java-Api-Rest
Java's API Rest use Sprint / Hibernate. Simple list Instructor's data and Instructor's courses.
The Data Base is H2

#Verbs HTTP
##GET /instructors/{username}
Get json from instructor to search
###Request
none
###Response
{
"courses": [],
"id": 1,
"username": "emartinez"
}
##GET /instructors 
Get List Intructors
###Request
none
###Response
List to Instructors in JSON's format

##GET /{username}/courses
Get list a courses from Instructor

###Request
None

###Response
List of courses in JSON's format
[{"id": 1,"description": "Risk Managment"}]


##POST /instructors
Insert new instructor
###Request
{
"username":"emartinez",
"password":"123"
}
###Reponse
201 Created

##POST /{username}/courses
Create new course from Instructor

###Request
{
"instructor":"emartinez",
"description":"Risk Managment"
}

###Response
201 Created

#Comands
To build : gradle bootrun
