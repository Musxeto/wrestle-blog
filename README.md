# Wrestle Pro Blog

## Overview
Wrestle Pro Blog is a web project built with Flask, a Python web framework. This project serves as a platform for creating and managing blog posts related to professional wrestling. Users can view blog posts, access the about page, contact the administrators, and log in to the dashboard for managing blog content.

## Technologies Used
- Flask: Web framework for Python
- SQLAlchemy: Object-Relational Mapping (ORM) for database interaction
- Flask-Mail: Extension for sending emails
- HTML, CSS: Frontend development
- Bootstrap 5: Frontend framework for responsive design

## Features
1. **Homepage (`/`):**
   - Displays a list of blog posts with pagination.
   - Navigation to the previous and next pages.

2. **Individual Post (`/post/<string:post_slug>`):**
   - Displays a detailed view of a specific blog post.

3. **About Page (`/about`):**
   - Provides information about Wrestle Pro.

4. **Dashboard (`/dashboard`):**
   - Requires authentication (username and password) to access.
   - Allows administrators to view and manage blog posts.
   - Edit and delete existing posts.
   - Add new posts.

5. **Login Page (`/dashboard`):**
   - Allows administrators to log in to the dashboard.

6. **Edit Page (`/edit/<string:sno>`):**
   - Allows administrators to edit existing blog posts or add new ones.

7. **Logout (`/logout`):**
   - Logs out the administrator.

8. **Delete Post (`/delete/<string:sno>`):**
   - Allows administrators to delete a specific blog post.

9. **Contact Page (`/contact`):**
   - Users can submit a contact form.
   - Sends an email to the administrator and a confirmation email to the user.
   - Saves form data to the database.

## Setup
1. Clone the repository: `git clone https://github.com/your-username/your-repo.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Set up the database: Run `python` in the terminal and execute the following commands:
    ```python
    from main import db
    db.create_all()
    exit()
    ```
4. Create a `config.json` file with the required parameters.

## Running the Application
- Execute `python main.py` in the terminal.
- Access the application at `http://localhost:5000` in your web browser.

## Configuration
Modify the `config.json` file to customize parameters such as database URI, email settings, and administrator credentials.

## Contribution
Feel free to contribute by submitting issues or pull requests.

## License
This project is licensed under the [MIT License](LICENSE).
