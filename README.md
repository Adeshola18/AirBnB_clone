
AirBnB_clone
AirBnB clone is an ALX project to build an application similar tothe popular Airbnb. This application will be completed in milestones (steps) and each step will link to a concept:

## Description :house:

AirBnB is a complete web application, integrating database storage, 
a back-end API, and front-end interfacing in a clone of AirBnB.

The project currently only implements the back-end console.


## Storage :baggage_claim:

The above classes are handled by the abstracted storage engine defined in the 
[FileStorage](./models/engine/file_storage.py) class.

Every time the backend is initialized, HBnB instantiates an instance of 
`FileStorage` called `storage`. The `storage` object is loaded/re-loaded from 
any class instances stored in the JSON file `file.json`. As class instances are 
created, updated, or deleted, the `storage` object is used to register 
corresponding changes in the `file.json`.

## Console :computer:

The console is a command line interpreter that permits management of the backend 
of cloneBnB. It can be used to handle and manipulate all classes utilized by 
the application (achieved by calls on the `storage` object defined above).

### Using the Console

The AirBnB console can be run both interactively and non-interactively. 
To run the console in non-interactive mode, pipe any command(s) into an execution 
of the file `console.py` at the command line.

### Files and Directories
models: This directory contains all classes used for the entire project. A class, called "model" in a OOP project is the representation of an object/instance.

tests: This directory contains all unit tests.

console.py: console.py file is the entry point of our command interpreter

models/base_model.py: This file is the base class of all our models. It contains common elements:

attributes: id, created_at and updated_at
methods: save() and to_json()
models/engine: This directory contains all storage classes (using the same prototype). For the moment, it contains onlt the file_storage.py file.

## Authors :black_nib:
* **Timothy Atobatele** <[Adeshola18](https://github.com/Adeshola18)>
* **Yusuf Simpa** <[yusim2020](https://github.com/yusim2020)>
