# Background
The project is a simple copy of the AirBnB website.
 
Airbnb: is an online accommodation booking solution for short and long term stay for travelers all over the world. It enables people travelling on budget to find decent and homely accommodation.
It allows not only hotels but also home owners/families with extra space to list their properties and charge a fraction of the standard costs.
 
If features only some of the fundamental concepts of the higher level programming track.
Like:
A command interpreter to manipulate data without a visual interface, like in a Shell (perfect for development and debugging)
A website (the front-end) that shows the final product to everybody: static and dynamic
A database or files that store data (data = objects)
An API that provides a communication interface between the front-end and your data (retrieve, create, delete, update them)
 
# Concepts to follow:
Unittest
Python packages
Serialization/Deserialization
*args, **kwargs
datetime
More coming soon!
 
# Steps
The application is built in multiple step.
Each step links to a concept:
The console
Web static
MySQL storage
Web framework - templating
RESTful API
Web dynamic
 
# Files and Directories
models directory contains all classes used for the entire project. A class, called “model” in a OOP project is the representation of an object/instance.
tests directory contains all unit tests.
console.py file is the entry point of our command interpreter.
models/base_model.py file is the base class of all our models. It contains common elements:
attributes: id, created_at and updated_at
methods: save() and to_json()
models/engine directory contains all storage classes (using the same prototype).
 
# Storage
In this project, manipulates 2 types of storages: file and database.
Separate “storage management” from “model” to make the models modular and independent. With this architecture, you can easily replace your storage system without re-coding everything everywhere.
We use class attributes for all objects
 
File storage == JSON serialization
Here, we write in a file all objects/instances created/updated in the command interpreter and restore them when it starts.

