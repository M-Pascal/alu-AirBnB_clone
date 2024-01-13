# AirBnB Console project description:
The objective of this project is to deploy a simplified version of the AirBnB website on a server. While it will not encompass all the features of the original platform, it will encompass enough fundamental concepts to serve as a foundation for higher-level programming as we enhance our learning experiance.

# What is a command Interpreter?
Think of it as similar to the Shell, but tailored to a specific use-case. In our context, we aim to manage the objects within our project with the following capabilities:

Create a new object (e.g., a new User or a new Place)
Retrieve an object from a file, a database, etc.
Perform operations on objects (e.g., counting, computing statistics, etc.)
Update attributes of an object.
Delete an object.

# Steps that will taken to Develop a Command Interpreter for Managing AirBnB Objects
This initial step holds significant importance as it lays the groundwork for subsequent projects, including HTML/CSS templating, database storage, API integration, and front-end development. Steps are:
The console: this where we create objects, it will help undertand serialization/deserialization and created our first stotage as well.
HTML file for making application pretty and creating visual interface for future user.
MySQL where we will be dealing with difference type of storage (Data Base).
Deployment of HTML with fabric will help us to put all things we made on the servers.
The flask web application server where we will taking model that are in storage and we will be able to intergrate it with HTML.
RestAPI where take object and we can put them in the into JSON.
Dynamic where we can talke JSON API and we intregrate it with HTML so that we can be able to share our web application we have developed (AirBnB).

# Running the Console
You can utilize the console in both interactive and non-interactive modes:
Interactive mode:
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$

Non-interactive mode (similar to the C Shell project):
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$

# Supported Commands
create - Create an object
show - Display an object based on its ID
destroy - Delete an object
all - Show all objects, either of one specific type or all types
update - Modify an instance based on the class name and ID
quit/EOF - Exit the console
help - Obtain descriptions of available commands
To initiate the console, use the following command in your shell:
AirBnB_clone$ ./console.py
(hbnb) 

# Create
To create an object, use the following format: "create " (e.g., create BaseModel).
(hbnb) create BaseModel

# Show
To display an instance based on its class name and ID, use the following format:
(hbnb) show BaseModel 1234-1234-1234

# Destroy
To delete an instance of an object, use the format: "destroy " (e.g., destroy BaseModel 1234-1234-1234).
(hbnb) destroy BaseModel 1234-1234-1234

# All
To list all objects of a specific class or all classes, use one of the following formats:
(hbnb) all
(hbnb) all State

# Update
To update an instance based on its class name and ID, use the following format:
(hbnb) update BaseModel 1234-1234-1234 email "aibnb@holbertonschool.com"

# Quit
To exit the console, type "quit" or use the EOF (End of File) command.

# Help
To get information about a specific command or see a list of available commands, use the "help" command followed by the command name (e.g., help quit).
(hbnb) help quit
Defines quit option
(hbnb)

# Supported classes
BaseModel
User
State
City
Amenity
Place
Review

# Authors
Pascal Mugisha - P.mugisha@alustudent.com
