# cpsc449midtermproject_issac
## Team Member
- **Name**: Issac Zhou
- **CWID**: 885251249
- **Email**: issaczhou@csu.fullerton.edu
- **Team Members**: 1 (Issac Zhou only)


## Project Overview

This project is a RESTful API developed using the Flask framework, including features such as error handling, authentication, file handling, and implementation of public and admin routes. It covers common CRUD operations to ensure understanding of how to build a robust API system.

Key features of the project include:
- **Error Handling**: Return standardized error messages and status codes for different types of errors.
- **Authentication**: Protect admin routes using JSON Web Token (JWT) for user login.
- **File Handling**: Allow users to upload files with validation for file type and size.
- **Public and Admin Routes**: Provide public routes that do not require authentication, while admin routes require authentication.

The purpose of this project is to help developers learn how to use Flask to build a robust API that includes error handling, authentication, and file upload functionality.

## Running the Project

### 1. Clone the Project Code
```bash
git clone https://github.com/1172351840/cpsc449midtermproject_issac.git
```

### 2. Create and Activate a Virtual Environment

Navigate to the project directory, then create and activate a Python virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Project Dependencies

After activating the virtual environment, install the required dependencies:

```bash
pip install -r requirements.txt
```

### 4. Run the Flask Application

With the virtual environment activated and all dependencies installed, start the Flask application:

```bash
python3 main.py
```

The application will run by default at `http://127.0.0.1:5000`.

## Testing with Postman

### 1. Log In and Get a JWT Token
- **Request Type**: `POST`
- **URL**: `http://127.0.0.1:5000/login`
- **Body (JSON)**:
  ```json
  {
    "username": "test_user",
    "password": "test_password"
  }
  ```
- **Response**: A JWT token will be returned upon successful login.

### 2. Access Protected Route
- **Request Type**: `GET`
- **URL**: `http://127.0.0.1:5000/protected`
- **Authorization**: Select `Bearer Token` and paste the JWT token from the previous step.

### 3. Upload a File
- **Request Type**: `POST`
- **URL**: `http://127.0.0.1:5000/upload`
- **Body (form-data)**:
  - `Key`: `file`  
  - `Value`: Select a valid file (e.g. `.png`, `.jpg`, `.pdf`)

### 4. Access Public Information
- **Request Type**: `GET`
- **URL**: `http://127.0.0.1:5000/public`

### 5. Add a New User
- **Request Type**: `POST`
- **URL**: `http://127.0.0.1:5000/user`
- **Body (JSON)**:
  ```json
  {
    "username": "new_user",
    "password": "new_password"
  }
  ```

## Project Files
- **`main.py`**: The main application file containing all routes and functionality.
- **`config.py`**: Stores application configuration.
- **`requirements.txt`**: Lists all project dependencies.
- **`README.md`**: Project description and usage guide.

- **`uploads/`**: Directory for storing uploaded files.

## Demo Video
This project includes a demo video that showcases key API functionalities such as authentication and file upload. You can find the video (`demo_video_googledrivelink.txt`) on the project's GitHub repository link through Google Drive.


## Submission Requirements
The project has been submitted to the GitHub repository, including the following:
- All code files for the Flask project.
- Demo video link
- WordDoc of all the PostMan testing screenshots
- Complete the `README` file.

If you have any questions, please get in touch with me!

