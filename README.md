# AirBnB Clone - The Console

![image](https://github.com/Itzsammi/AirBnB_clone/assets/107357783/8188e490-b362-4edf-a8e0-afd521a61ee6)

Welcome to the AirBnB clone project!
  

## Getting Started

 
**What’s a command interpreter?**

Do you remember the Shell? It’s exactly the same but limited to a specific use-case. In our case, we want to

be able to manage the objects of our project:

  

- Create a new object (ex: a new User or a new Place)

- Retrieve an object from a file, a database etc…

- Do operations on objects (count, compute stats, etc…)

- Update attributes of an object

- Destroy an object

  

### Learning Objectives

  

## General

 - How to create a Python package
   
  - How to create a command interpreter in Python using the cmd module
   
   - What is Unit testing and how to implement it in a large project
   
   - How to serialize and deserialize a Class
   
   - How to write and read a JSON file
   
   - How to manage datetime
   
   - What is an UUID
   
   - What is *args and how to use it
   
   - What is **kwargs and how to use it
   
   - How to handle named arguments in a function

  
  

## Execution

  
Your shell should work like this in interactive mode:

  
```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF help quit

(hbnb)
(hbnb)
(hbnb) quit
$
```

But also in non-interactive mode: (like the Shell project in C)

```
$ echo "help" | ./console.py

(hbnb)

Documented commands (type help <topic>):
========================================

EOF help quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

  
Documented commands (type help <topic>):
========================================
EOF help quit
(hbnb)
$

```

## Usage Examples

**Launching the console**
```
$ ./console.py
(hbnb) 
```
**Creating a new object**
```
(hbnb) create
** class name missing **
(hbnb) create User
53ef7f85-1e90-4c8a-927f-751bcb386708
```
**Show an object**
```
(hbnb) show User
** instance id missing **
(hbnb) show User 53ef7f85-1e90-4c8a-927f-751bcb386708
[User] (53ef7f85-1e90-4c8a-927f-751bcb386708) {'id': '53ef7f85-1e90-4c8a-927f-751bcb386708', 'created_at': datetime.datetime(2024, 3, 18, 10, 8, 47, 373063), 'updated_at': datetime.datetime(2024, 3, 18, 10, 8, 47, 373072)}
```
**Update an object**
```
(hbnb) all
["[User] (53ef7f85-1e90-4c8a-927f-751bcb386708) {'id': '53ef7f85-1e90-4c8a-927f-751bcb386708', 'created_at': datetime.datetime(2024, 3, 18, 10, 8, 47, 373063), 'updated_at': datetime.datetime(2024, 3, 18, 10, 8, 47, 373072)}"]
(hbnb) update
** class name missing **
(hbnb) update User
** instance id missing **
(hbnb) update User 53ef7f85-1e90-4c8a-927f-751bcb386708
** attribute name missing **
(hbnb) update User 53ef7f85-1e90-4c8a-927f-751bcb386708  Age "20"
(hbnb) all
["[User] (53ef7f85-1e90-4c8a-927f-751bcb386708) {'id': '53ef7f85-1e90-4c8a-927f-751bcb386708', 'created_at': datetime.datetime(2024, 3, 18, 10, 8, 47, 373063), 'updated_at': datetime.datetime(2024, 3, 18, 10, 8, 47, 373072), 'Age': '36'}"]
(hbnb)
```
**Destroy an object**
```
(hbnb) destroy
** class name missing **
(hbnb) destroy User
** instance id missing **
(hbnb) destroy User 53ef7f85-1e90-4c8a-927f-751bcb386708
(hbnb)
```
