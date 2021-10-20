# RescueAnimalApplication
Dash-Py-Mongo Full Stack Application

Ryan Helferich

About the Project/Project Title
As part of Global Rain, a leading software company, we were tasked with developing the latest application for Grazioso Salvare, a company that identifies dog candidates for search and rescue training. This project uses existing data from various animal shelters to identify and categorize dogs. This application was developed to be a full-stack solution for the company, fitting all their data handling needs while providing an essential front-end interface for the employees to use with ease. While provided with a database, we wanted the most efficient methods for handling and manipulating the data. This project utilizes the Model-View-Controller software design that allows us to maintain the simplistic functionality between the user, controller, and the data model. In the backend of the application, we begin our manipulation of the data with Mongo DB. Our front-end system is created through Dash, an open-source Python framework for quick analytical applications. Finally, we connect both Mongo and Dash through a custom Python module that provides a quick usage of functionality to gather the data we need and send it back to the user as soon as possible. 

Motivation
MongoDB is fast and efficient NoSQL database program that powers our backend with direct access to the data. This program utilizes JSON based formatting to store documents, which can in turn handle high volume loads allowing the application to scale both vertically and horizontally. Dash is an open-source Python framework, commonly used for analytical web applications, that allows for the simplification of a front-end interface through our data driven system. We connect everything through Python, allowing easy to use dynamic typing capabilities and an efficient way to connect multiple areas of a web application. 
Getting Started
To get started with this project, you must first install a local copy of the entire project to begin. You will need to ensure you have Mongo DB installed on your system, as well as the latest Python version. Once your project is laid out correctly, we can begin by setting up access to the database. You’ll want to use your current terminal to create a new Mongo database and Import the CSV file containing the company data. Finally, you must ensure you create a user with access to this database containing read and write permissions. Below is a helpful link for those entirely new to MongoDB, or if you’re experienced and need a refresher. 

https://docs.mongodb.com/manual/tutorial/create-users/

Installation
The tools you will need installed are:
		Backend – MongoDB
		https://docs.mongodb.com/manual/installation/

		Frontend – Dash Framework
		https://dash.plotly.com/installation

		Python
		https://www.python.org/downloads/

		JupyterLab
		https://jupyter.org/install	

CRUD OPERATIONS
The project at hand can handle all four basic CRUD operations on the database. With MongoDB, we can create documents, read from the database, update an individual or multiple documents, while also having the ability to delete a single or multiple sets of documents at once. The update and delete methods in the module can take in a third parameter known as “count” which can determine if a single or multiple amounts of documents are needing to be operated on. 

Next Steps
After installing all the required software, creating a database with a new user, and testing the application with the Python Module Test script, we can continue onto the front-end interfacing of the project. You will need to have the Dash framework installed as stated above and will now run Jupyter with the ‘DashBoard.ipynb’ file. This file utilizes the connections between MongoDB and the PyMongoModule (connector) to give us an efficient front-end system to read, write, update, and delete data from the database properly for any user. 
 
Reminders
	There are a few things to note and remember if you begin to get stuck anywhere in the process of using the application, entirely based on my experience developing it. When accessing the database, whether its through the test module or through the Dashboard file, ensure your terminal is running the Mongo Server in the background. You can check by using the ‘status’ command in Mongo. If you are sure your server is running but still cannot connect to the database, triple check your username and password in the Dashboard file as well as the connection to the database in the ‘PyMongoModule’ file. If the connection is not setup correctly with your credentials, it will never have access.

The Dash Framework
Dash is our primary front-end framework in this application since it provides a large and powerful library for simplifying our data driven application. This allows us to create the tables and widgets for us to filter, view and sort our data on the user end. Each of the filters and widgets is linked to a query when selected that allows our Python module to trigger a request into the database, bringing out desired information to the surface. While this application is primarily structure in a model-view-controller architecture, our Dash framework is essentially the view and controller portion as it allows us to view our data and manipulate it. Since we use MongoDB in our application, with its document-oriented database, we can easily filter and sort through our entire database and bring it directly into view for our user in Dash. 

Using the Application
Once the database is setup and running, begin by running the Dashboard portion of the project. When the Dashboard has fully initialized, it will connect through our Python module and access the database directly. From here our system will begin to query and read the database, sorting it into its appropriate tables for us to view the data as seen below. 
 
Once all the data has been loaded into the dashboard from the database, we can then filter and select individual types of animals. We can filter between water rescue, mountain or wilderness, disaster or individual and then reset all the filters back to normal. Each of the widget-based filters allows us to direct our search to the individual type of rescue animal we will need to look for. Once we filter the type we need, we can then select up to five animals individually with the check box widgets on the left side of the data in the table. When we select the desired filter, we can then see our graph and geographical map change with the selected information. The pie chart graph shows us each percentage that makes up the filtered set of data, identifying the animal types and their relation to how many it consists of. Finally, after we filter our choice of rescue type, we can select up to five of the individual animals. The geographical map will then create a marker on the location of those five animals selected. This marker is clickable and will show the animals information as well as their location. Below are examples of the graphs and the filters for animal rescue types being applied. 
     
Contact
Ryan Helferich: Lead Developer

Module 8 Prompt
    How do you write programs that are maintainable, readable, and adaptable? Especially consider your work on the CRUD Python module from Project One, which you used to connect the dashboard widgets to the database in Project Two. What were the advantages of working in this way? How else could you use this CRUD Python module in the future?
    How do you approach a problem as a computer scientist? Consider how you approached the database or dashboard requirements that Grazioso Salvare requested. How did your approach to this project differ from previous assignments in other courses? What techniques or strategies would you use in the future to create databases to meet other client requests?
    What do computer scientists do, and why does it matter? How would your work on this type of project help a company, like Grazioso Salvare, to do their work better?
    
    In order to maintain a program, the functionality and modularity must remain current. The first example of allowing the project itself to be reusable or modular was based on our Python module allowing us to connect between the database and the dashboard. The primary advantage of developing the module was being able to deploy it into various projects or allowing us to include additional databases in this single project. As a computer scientist, its essential to approach a problem by identifying the desired outcome and then determining the correct stack,tools or development style to achieve that same outcome. In the Grazioso project, we initially were given a large set of data and needed to create a complete application to access and modify it. The first approach to this was thinking of how the application should be designed in order to compliment the users experience for using the data set efficiently. We then determined the most efficient and modular solution for the company, a basic python module for handling the database and followed it up with a python framework known as Dash for the front end. The code itself was consistent and utilized python through the entire application. I would use the same initial strategy of understanding the company and what it desires in additional projects, and possibly pivot into another framework or language depending on the scenario. Computer scientiist identify and solve problems through efficient and effectives means. Instead of relying on human capstones or the inability to conquer a task, computer science principles are used to tackle any task in the fastest way possible. 

