LittleLemon Project
Overview

LittleLemon is a web and mobile application designed to streamline table booking for the Little Lemon restaurant. Built with Django and MySQL, this project offers a robust backend API that allows users to view available booking times and make reservations.
Features

    API Integration: Built a RESTful API to handle table booking operations, including creating, reading, updating, and deleting bookings.

    Database Integration: Connected the backend to a MySQL database, ensuring seamless data synchronization.

    User Interface: Developed dynamic templates for displaying available booking times, enhancing the user experience.

Technologies Used

    Backend: Django

    Database: MySQL

    Frontend: HTML, CSS, JavaScript (or any frameworks you used for the frontend)

    Version Control: Git, GitHub

Setup and Installation

    Clone the repository:

git clone https://github.com/shahrzadbst/Littlelemon.git

Install dependencies:

pip install -r requirements.txt

Set up the MySQL database and configure the connection in settings.py.

Run migrations to set up the database:

python manage.py migrate

Start the Django development server:

    python manage.py runserver

API Endpoints
1. Restaurant Routes

    GET /restaurant/: Retrieves information about the restaurant.

2. Menu Routes

    GET /restaurant/menu/: Returns the menu items available at the restaurant.

3. Booking Routes

    GET /restaurant/booking/: Retrieves the current booking status and available booking slots for the restaurant.

    POST /restaurant/booking/: Allows users to create a new booking.

4. Tables Routes

    GET /restaurant/booking/tables/: Provides the available tables for the restaurant.

5. User Authentication Routes

    POST /auth/users/: Registers a new user for the restaurant application.

    POST /auth/token/login: Logs in a user and returns an authentication token.

    POST /auth/token/logout: Logs out a user by invalidating their authentication token.

This gives a more structured breakdown of the different API endpoints in your project, making it easier for others to understand how your application handles bookings, restaurant data, and user authentication.
Example API Flow:

    User Registers: The user calls POST /auth/users/ to create an account.

    User Logs In: The user logs in via POST /auth/token/login to receive an authentication token.

    View Menu: The user can view the menu by calling GET /restaurant/menu/.

    Check Available Booking Times: The user checks available booking slots via GET /restaurant/booking/ or checks available tables with GET /restaurant/booking/tables/.

    Make a Booking: Finally, the user can make a booking by calling POST /restaurant/booking/ with the appropriate details.