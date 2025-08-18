# Build REST APIs with Django REST Framework and Python

## Course Link

[https://www.udemy.com/course/django-rest-framework](https://www.udemy.com/course/django-rest-framework)

## Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/valeriia-nedashkivska/udemy-imdb.git
    cd udemy-imdb
    ```

2. **Create and activate virtual environment**
    ```bash
    python -m venv venv
    # On Linux/Mac
    source venv/bin/activate
    # On Windows
    venv\Scripts\activate
    ```

3. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**
    - Create a `.env` file from `.env.example`:
       ```bash
       # On Linux/Mac
       cp .env.example .env      
       # On Windows 
       copy .env.example .env   
       ```
    - Generate a `SECRET_KEY`:
       ```bash
       python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())" 
       ```
      Copy the key and paste it into the `.env` file, replacing `###`.

5. **Apply migrations**
    ```bash
    python manage.py migrate
    ```

6. **Create superuser (optional, for admin access)**
    ```bash
    python manage.py createsuperuser
    ```

7. **Run the development server**
    ```bash
    python manage.py runserver
    ```