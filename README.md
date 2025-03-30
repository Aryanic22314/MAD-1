Author 
Aryan mishra
23f1002447
23f1002447@ds.study.iitm.ac.in 
I am Aryan mishra, currently in the Diploma Level of BS Degree,
Description 
The Quiz Master V1 project is a multi-user web application designed for exam preparation. It 
allows admins to manage subjects, chapters, quizzes, and questions, while users can register, take 
quizzes, and view their scores. Built using Flask and SQLite, the app ensures secure 
authentication and dynamic database creation. 
Technologies Used 
● Backend: 
● Flask: Core framework for routing and application logic. 
● Flask-SQLAlchemy: ORM for managing database interactions. 
● SQLite: Lightweight database for storing application data. 
● Flask-Login: Handles user authentication and session management. 
● Flask-WTF: Simplifies form creation and validation. 
● Werkzeug: Provides secure password hashing. 
● Python-Dotenv: Manages environment variables securely. 
● Frontend: 
● Jinja2: Templating engine for generating dynamic HTML pages. 
● HTML/CSS/Bootstrap: For responsive and styled user interfaces. 
Purpose: These technologies were chosen for their simplicity, scalability, and ability to integrate 
seamlessly into a full-stack web application. 
DB Schema Design 
The database is structured with the following tables: 
1. 
User: Stores user details (e.g., email, password hash) with an is_admin flag for role-based 
access. 
2. Subject: Contains subject names and descriptions. 
3. Chapter: Links chapters to subjects via a foreign key. 
4. Quiz: Stores quiz details like title, chapter ID, date, and duration. 
5. Question: Holds quiz questions with options and correct answers. 
6. QuizAttempt: Tracks user attempts with scores and timestamps. 
7. 
Answer: Records user-selected options for each question. 
Reasons: The schema ensures logical relationships between entities (Subjects → Chapters → 
Quizzes → Questions) while maintaining data integrity through foreign keys. 
API Design 
APIs were implemented for managing subjects, chapters, quizzes, and users: 
● Example endpoints: 
● /api/subjects: Fetches all subjects as JSON data. 
● /api/quizzes/<id>: Retrieves details of a specific quiz. 
● Implementation was done using Flask routes with @app.route() decorators. 
A YAML file defining the API structure is included in the submission. 
Architecture and Features 
● The project follows an MVC (Model-View-Controller) architecture: 
● Models: Defined in app.py using SQLAlchemy ORM (e.g., User, Subject). 
● Controllers: Flask routes handle requests (e.g., /admin/dashboard). 
● Views: Jinja2 templates render dynamic HTML pages. 
Features Implemented: 
● Admin functionalities: 
● Manage users, subjects, chapters, quizzes, and questions. 
● View user performance analytics with summary charts. 
● User functionalities: 
● Register/login to take quizzes by subject or chapter. 
● View quiz results and performance analysis. 
Additional Features: Password hashing for security, responsive design using Bootstrap, and form 
validation with Flask-WTF. 
Video 
Admin Dashboard - Quiz Master.mp4

