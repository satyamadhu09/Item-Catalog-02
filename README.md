# Item-Catalog

## Application Overview:

This is an application representing the Item Catalog project  that provides a list of items within a variety of categories, as well as providing a user registration and authentication system. This project uses Google OAuth2 Client API for the user to sign in and authenticate to the application. All the code is written in python which uses Flask Web Framework with SQL alchemy.

## Requirements:

- HTML 
- CSS 
- Flask 
- SQL Alchemy and 
- Google OAuth2 API

## Softwares required:

- Python
- Vagrant 
- VirtualBox and 
- Vagrant Virutal Machine(VM)

## Steps followed:

1. Install Vagrant and VirtualBox
2. Launch the Vagrant VM by following commands:
  $ vagrant up
  $ vagrant ssh
  
3. Write your Flask application locally in the vagrant/catalog directory which will automatically be synced to /vagrant/catalog within the VM.

4. Now to initialize the database, firstly you need to run a file which will create a database to add data.
                   $   python database_setup.py

5. Adding some data to the initaialized database is a healthy process.

                   $   python lotsofmenus.py

6. Run your application within the VM  which is resided in your vagrant directory.

                   $   python ./application.py

7. To Use Google Authentication Services you need a .json file. You can create a project to avail Google's OAuth service by taking a  Client Id at:
		
	 https://console.developers.google.com

 After creating and downloading .json file, place it in the directory in which it is accessible to the main project file. Adding, editing, and deleting menu items requires the user to log in to the application. Users can only see all other items but can edit and delete their own items.

Access and test your application by visiting the below URL in your browser:
 
                          http://localhost:8000 
