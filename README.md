# Item Catalog

An application that provides a list of items within a variety of categories as well as provide a user registration and authentication system. Registered users will have the ability to post, edit and delete their own items.

![blog demo](https://github.com/anmolmann/Item-Catalog/blob/master/images/restaurants.png)

## Table of contents

- [Quick Start](#quick-start)
- [Documentation](#documentation)
- [Setup](#setup)
- [Usage](#usage)

## Quick Start

The Item Catalog project consists of developing an application that provides a list of items within a variety of categories, as well as provide a user registration and authentication system.
	- The homepage displays all current categories along with the latest added items.
	- Selecting a specific category shows you all the items available for that category.
	- Selecting a specific item shows you specific information of that item.
	- After logging in, a user has the ability to add, update, or delete item info.
	- The application provides a JSON endpoint, at the very least.

![blog demo](https://github.com/anmolmann/Item-Catalog/blob/master/images/menu.png)


## Documentation

This is a RESTful web application using the Python framework Flask along with implementing third-party OAuth authentication. Also, properly implementing authentication mechanisms and appropriately mapping HTTP methods to CRUD operations are core features of a properly secured web application.

## Setup

- Install Python.

- Install all the required packages first:
	- apt-get -qqy update
	- apt-get -qqy install postgresql python-psycopg2
	- apt-get -qqy install python-sqlalchemy
	- apt-get -qqy install python-pip
	- pip install werkzeug==0.8.3
	- pip install flask==0.9
	- pip install Flask-Login==0.1.3
	- pip install oauth2client
	- pip install requests
	- pip install httplib2

#### VirtualBox

VirtualBox is the software that actually runs the VM. [You can download it from virtualbox.org, here.](https://www.virtualbox.org/wiki/Downloads)  Install the *platform package* for your operating system.  You do not need the extension pack or the SDK. You do not need to launch VirtualBox after installing it.

**Ubuntu 14.04 Note:** If you are running Ubuntu 14.04, install VirtualBox using the Ubuntu Software Center, not the virtualbox.org web site. Due to a [reported bug](http://ubuntuforums.org/showthread.php?t=2227131), installing VirtualBox from the site may uninstall other software you need.

#### Fetch the Source Code and VM Configuration

**Windows:** Use the Git Bash program (installed with Git) to get a Unix-style terminal.  
**Other systems:** Use your favorite terminal program.

- From the terminal, run:
	- git clone https://github.com/anmolmann/Item-Catalog.git

- This will give you a directory named **Item-Catalog** complete with the source code.

## Usage

#### Run the virtual machine!

- Using the terminal, change directory to Item-Catalog (**cd Item-Catalog**)

#### Running the Restaurant Menu App

- Type **ls** to ensure that you are inside the directory that contains project.py, database_setup.py, and two directories named 'templates' and 'static'

- Now type **python database_setup.py** to initialize the database.

- Type **python lotsofmenus.py** to populate the database with restaurants and menu items. (Optional)

- Type **python project.py** to run the Flask web server.

- Access and test your application by visiting http://localhost:5000 locally
	- In your browser visit **http://localhost:5000** to view the restaurant menu app.  You should be able to view, add, edit, and delete menu items and restaurants.
