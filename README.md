# Java-Api-Rest
Java's API Rest use Sprint / Hibernate. Simple list Instructor's data and Instructor's courses.

#To build : gradle bootrun

#Verbs HTTP
## GET
### /instructors : Get List Intructors
### /
## POST
### /instructors : Insert new instructor
###Request
{
"username":"emartinez",
"password":"123"
}
###Reponse
201 Created
