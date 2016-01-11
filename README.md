Java-Api-Rest
===========

    Simple Java's API Rest for Instructor's data and Instructor's courses. Whith Java 8, Hibernate, Sprint, and H2


##Verbs HTTP



###GET /instructors/{username}

*Get Instructor in JSON's format.*


####Request

None

####Response
`{
"courses": [{"id": 1,"description": "Risk Managment"}],
"id": 1,
"username": "emartinez"
}`

###GET /instructors 

*Get Instructor's list*

####Request
none
####Response
`[{
"courses": [{"id": 1,"description": "Risk Managment"}],
"id": 1,
"username": "emartinez"
}]`

###GET /{username}/courses
Get list a courses from Instructor

###Request
None

###Response
Courses list in JSON's format  

`[{"id": 1,"description": "Risk Managment"}]`


##POST /instructors
Insert new instructor
###Request
{
"username":"emartinez",
"password":"123"
}
###Response
201 Created

##POST /{username}/courses
Create new course for Instructor

###Request
{
"instructor":"emartinez",
"description":"Risk Managment"
}

###Response
201 Created

##Comands
**To build** : gradle bootrun
**To publish** : gradle clean build


publish file war from build/libs/


#Demo

Publish in Elastic Beanstalk from AWS (Amazon)   [http://javademo.erikmartinez.mx](http://javademo.erikmartinez.mx)

----------

>  Based on the demo writen by  [Oscar Bernal](https://github.com/obernal) for  [PlatziJava](https://github.com/platzi/platziJava). 

> MarkDown written with [StackEdit](https://stackedit.io/).
