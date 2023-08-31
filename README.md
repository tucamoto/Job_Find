# Job_Find
find your job

Program Overview: Job Finder Web Application (For Educational Purposes)
This is an overview of the Job Finder web application's codebase, developed for educational purposes. The application is built using Node.js and Express.js for the backend, along with Handlebars for rendering dynamic HTML templates. The primary aim of this project is to provide a learning platform for understanding web application development concepts.
Backend (app.js):
1.	Required Dependencies: The application requires various dependencies including express, express-handlebars, path, body-parser, Sequelize, and others.
2.	Server Setup: The Express app is created, and the server listens on port 3000. A console log indicates that the server is running.
3.	Middleware Setup:
•	body-parser is used to parse incoming request bodies.
•	The express-handlebars templating engine is configured to render views.
•	A static folder for serving static files (e.g., CSS) is defined.
4.	Database Connection: The application establishes a connection to an SQLite database using Sequelize's ORM. A success or error message is logged.
5.	Routes:
•	The root route (/) handles job searching functionality.
•	The /jobs route uses the separate jobs.js router.
Frontend (HTML Views):
1.	index.html, add.html, and other view templates are provided.
2.	The templates use Bootstrap CSS for styling.
Views (Handlebars Templates):
1.	add.handlebars: This template provides a form for users to submit job listings.
2.	index.handlebars: This template displays job listings and includes a search form.
3.	views.handlebars: This template displays detailed information about a job.
Routes (routes/jobs.js):
1.	/test: A test route that responds with "Ok".
2.	/view/:id: Retrieves a job by ID and renders the view.handlebars template.
3.	/add: Renders the add.handlebars template for posting new jobs.
4.	/add (POST): Handles the submission of a new job, creating a job record in the database.
Model (models/Job.js):
1.	Job Model: Defines the structure of a job using Sequelize. The attributes include title, description, salary, company, email, and new_job.
Database Connection (db/connection.js):
1.	Sequelize Setup: Creates a connection to an SQLite database (app.db).
This codebase serves as a practical learning resource for understanding key concepts related to web application development. It offers insights into the development of CRUD operations, routing, database interactions, and templating using a model-view-controller (MVC) architecture.

