AirBnB clone - The console
This project is the first stage on building a clone of the AirBnB website. This stage implements a backend interface, or console, to manage program data, and the console commands allow the user to create, update, destroy ... objects, and manage file storage. Using a system of JSON serialization/deserialization.

How to Use
After cloning the repository locate the "console.py" file and run it
AirBnB_clone$ ./console.py
Then a promp will appear like this

(hbnb)
Now u can Use our built in commands

Commands
command	Description	Usage
EOF	the EOF exits the program	EOF
all	Prints all string representation of all instances based or not on the class name	all
count	counts how many instances of class created and saved	count <class_name>
create	creates a new instance of the class passed as argument	create
destroy	Deletes an instance based on the class name and id	destroy
help	List available commands with "help" or detailed help with "help cmd"	help
quit	The quit command exits the program	quit
show	prints the string representation of an instance	show
update	Updates an object's attributes	update
Alternative Syntax
Also you can run the commands [count, show, destroy, update, all] in this format too:

<class name>.<command>([<id> [<*args> or <**kwargs>]])
Examples
Syntax 1
Create Object
Usage: create <class_name>

(hbnb) create User
cb8562e5-82c1-4cb8-9d58-06c0fe3e0c98
(hbnb)  
Show string represenation of an object
Usage: show <class_name> <_id>

(hbnb) show User cb8562e5-82c1-4cb8-9d58-06c0fe3e0c98
[User] (cb8562e5-82c1-4cb8-9d58-06c0fe3e0c98) {'id': 'cb8562e5-82c1-4cb8-9d58-06c0fe3e0c98', 'created_at': datetime.datetime(2021, 11, 9, 17, 8, 45, 23018), 'updated_at': datetime.datetime(2021, 11, 9, 17, 8, 45, 23018)}
(hbnb) 
Destro object
Usage: destroy <class_name> <_id>

(hbnb) destroy User cb8562e5-82c1-4cb8-9d58-06c0fe3e0c98
(hbnb) show User cb8562e5-82c1-4cb8-9d58-06c0fe3e0c98
** no instance found **
(hbnb) 
