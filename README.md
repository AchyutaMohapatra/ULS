# ULS
A URL shortener web application
<br>
<br>
## Description <br>
ULS is a URL-shortening service developed using Python and Flask frameworks. It allows you to shorten long URLs into compact and shareable links. With ULS, you can easily create shorter and more manageable URLs for sharing on social media platforms, email, or any other medium.
<br>
<br>
## How to Run the Project <br>
To run the project, follow these steps:
<br>
1. Clone the repository: `git clone <repository_url>` <br>
2. Navigate to the project directory: `cd ULS` <br>
3. Install the dependencies: `pip install -r requirements.txt` <br>
4. Run the application: `python app.py`<br>
5. Access the application in your web browser at: `http://localhost:8000` 
<br>
Note: Make sure you have Python and Flask installed on your system before running the project.
<br>
<br>
## Tech Stack Used <br>
ULS is built using the following technologies:
<br>
- Python: A powerful programming language used for backend development.<br>
- Flask: A lightweight web framework for Python.<br>
- Bootstrap 5: A popular CSS framework for building responsive and stylish web interfaces.<br>
- CSS: Cascading Style Sheets for customizing the application's appearance.<br>
- SQLite: A lightweight and embedded database storing URL and statistics data.<br>
- Azure: Used for deployment of website 
<br>
<br>
## The Working <br>
- The application uses SQLite as the database to store URL data and user information. <br>
- It utilizes the Flask framework, along with other packages like hashids for generating short aliases, Flask-Login for user authentication, and Werkzeug for password hashing.<br>
- The application consists of several routes:<br>
  - `/`: The main route where authenticated users can shorten URLs. It handles both GET and POST requests. When a POST request is received, it checks if the URL is already present in the database and updates it if necessary. If it's a new URL, it generates a short URL and saves it in the database.<br>
  - `/register`: Handles user registration. It saves the username and hashed password in the database.<br>
  - `/login`:  Handles user login. It compares the provided username and password with the stored values in the database, and if they match, logs the user in.<br>
  - `/logout`: Logs out the currently authenticated user.<br>
  - `/<alias>`: Redirects the user to the original URL associated with the provided alias.<br>
  - `/stats`: Displays the statistics for the URLs created by the currently authenticated user.<br>
  - `/search`: Allows users to search for URLs based on notes, original URLs, or aliases which the shorten before.<br>
  - `/about`: Displays information about the application and its author.<br>
<br>
- The application utilizes templates (index.html, register.html, login.html, stats.html, search.html, about.html) to render HTML pages with dynamic content.<br>
- User authentication is handled using the User class, which extends the UserMixin class from Flask-Login. It provides methods for loading users from the database and managing user sessions.<br>
- Flash messages are used to display notifications and error messages to the user.<br>
- The application runs on the local development server when the script is executed directly.
<br>
<br>
## Key Takeaways <br>
- Building a URL shortener using Python and Flask.<br>
- Working with SQLite database for storing URL and user data.<br>
- User authentication and session management using Flask-Login.<br>
- Using Bootstrap and CSS for styling the web interface.<br>
- Handling form submissions and data validation.<br>
- Implementing search functionality to filter URLs based on keywords.<br>
<br><br>
## References<br>
- https://flask.palletsprojects.com/en/2.3.x/<br>
- https://getbootstrap.com/docs/5.0/getting-started/introduction/<br>
- https://www.sqlite.org/index.html<br>
- https://www.w3schools.com/<br>
- https://www.youtube.com/@CodeWithHarry<br>
- https://chozinthet20602.medium.com/authentication-with-flask-login-5d504af3f517<br>

<br>
<br>

##Demo Link <br>
- https://drive.google.com/file/d/16F00YYepCtWQZZz-seRiMvuvwEb5y3G9/view?usp=drivesdk
 
