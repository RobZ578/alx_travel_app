# ALX Travel App

A real-world Django project for a travel listing platform. This project serves as the foundation for building APIs and managing travel listings, with a focus on best practices for backend development, database management, and API documentation.

## Features

- Django backend with a modular app structure.
- MySQL database integration.
- REST API development using Django REST Framework.
- Cross-Origin Resource Sharing (CORS) enabled.
- Swagger and ReDoc API documentation via `drf-yasg`.
- Environment variables for secure and scalable configurations.
- Prepared for background tasks using Celery (RabbitMQ).

## Project Structure

alx_travel_app/
│── manage.py
│── requirements.txt
│── .gitignore
│── .env # not committed
│
├── alx_travel_app/
│ ├── settings.py
│ ├── urls.py
│ └── ...
│
├── listings/
│ ├── views.py
│ ├── urls.py
│ ├── models.py
│ └── ...

bash
Copy code

## Installation

1. **Clone the repository**
```bash
git clone https://github.com/RobZ578/alx_travel_app.git
cd alx_travel_app
Create a virtual environment

bash
Copy code
python -m venv tutorial-env
source tutorial-env/bin/activate    # Mac/Linux
tutorial-env\Scripts\activate       # Windows
Install dependencies

bash
Copy code
pip install -r requirements.txt
Set up environment variables
Create a .env file in the project root:

ini
Copy code
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_NAME=alx_travel
DATABASE_USER=root
DATABASE_PASSWORD=yourpassword
DATABASE_HOST=localhost
DATABASE_PORT=3306
Run database migrations

bash
Copy code
python manage.py migrate
Create a superuser

bash
Copy code
python manage.py createsuperuser
Run the development server

bash
Copy code
python manage.py runserver
API Documentation
Swagger UI: http://127.0.0.1:8000/swagger/

ReDoc: http://127.0.0.1:8000/redoc/

Test endpoint: GET /api/listings/hello/ returns:

json
Copy code
{
  "message": "Hello, ALX Travel App!"
}
Contributing
Make sure .env and virtual environments (venv) are not pushed to GitHub.

Follow Python/Django best practices when adding features.
