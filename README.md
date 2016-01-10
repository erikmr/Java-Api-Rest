# Java-Api-Rest
Java's API Rest use Sprint / Hibernate. Simple list Instructor's data and Instructor's courses.
The Data Base is H2

#Verbs HTTP
##GET /instructors 
Get List Intructors
###Request
none
###Response
List to Instructors in JSON format

##POST /instructors
Insert new instructor
###Request
{
"username":"emartinez",
"password":"123"
}
###Reponse
201 Created

#Comands
To build : gradle bootrun
