----------

# Learning Management System (LMS) Backend

The **Learning Management System (LMS)** backend is built using Django and Django REST Framework (DRF). It provides a robust API for managing users, courses, batches, groups, and other essential functionalities of the LMS.

----------

## Features

-   **User Authentication**: Registration, login, logout, password management
-   **Course Management**: Create, update, list courses
-   **Batch and Group Management**
-   **Student and Teacher Management**
-   **API Documentation**: Easy-to-reference API documentation

----------

## Technologies Used

-   **Python 3.x**
-   **Django**
-   **Django REST Framework**
-   **PostgreSQL** (or any other database of your choice)
-   **JWT** for authentication

----------

## Installation

### Prerequisites

-   Python 3.x installed on your machine
-   Virtual environment (recommended)
-   PostgreSQL (or any other database)

### Steps to Set Up

1.  **Clone the Repository:**
    
   
    
    `git clone <repository-url>
    cd lms_project/learning_mngt_system` 
    
2.  **Create a Virtual Environment:**
    
    
    
    ``python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate` `` 
    
3.  **Install Dependencies:**
    
 
    
    `pip install -r requirements.txt` 
    
4.  **Set Up the Database:**
    
    -   Configure your database settings in `settings.py`.
5.  **Run Migrations:**
   
    
    `python manage.py migrate` 
    
6.  **Create a Superuser (Optional):**
    

    
    `python manage.py createsuperuser` 
    
7.  **Run the Server:**
    
  
    
    `python manage.py runserver` 
    

----------

## API Documentation

Refer to the API documentation for detailed information on available endpoints, request formats, and responses.

----------

### Authentication Endpoints

-   **Register User**: `/register/`
-   **Login User**: `/login/`
-   **Change Password**: `/change-password/`
-   **Logout User**: `/logout/`
-   **Get User Profile**: `/profile/`
-   **Refresh Token**: `/token/refresh/`
-   **Get Total Users**: `/total_users/`
-   **List Users**: `/users/`

### Course Endpoints

-   **Create Course**: `/create/`
-   **Create Module**: `/create_module/`
-   **Add Material to Module**: `/add_material_to_module/`
-   **List Courses**: `/list/`
-   **Create Batch**: `/create_batch/`
-   **Update Batch**: `/update_batch/<int:batch_id>/`
-   **Create Group**: `/create_group/`
-   **Update Group**: `/update_group/<int:group_id>/`
-   **List Batches**: `/list_batches/`
-   **List Groups**: `/list_groups/`
-   **Add Student to Batch**: `/add_student_to_batch/<int:batch_id>/`
-   **Add Course to Batch**: `/add_course_to_batch/<int:batch_id>/`
-   **Get Total Batches**: `/get_total_batches/`

### Student Endpoints

-   **Create Student**: `/create/`

### Teacher Endpoints

-   **Create Teacher**: `/create_teacher/`

----------

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or features.


