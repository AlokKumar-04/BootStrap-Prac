# Django Bootstrap Carousel and ScrollSpy Example

This is a simple HTML template using Bootstrap 5 to demonstrate a carousel and ScrollSpy functionality within a Django project.

## Features

- **Bootstrap Navbar**: A responsive navbar with dropdown and navigation links.
- **Bootstrap Carousel**: A slideshow of images with captions.
- **ScrollSpy**: Automatically highlights navigation items as you scroll through sections on the page.

## Requirements

- Python 3.x
- Django 
- Bootstrap 5 (included via CDN)

## Setup

1. **Install Django** (if you haven't already):

    ```bash
    pip install django
    ```

2. **Create a Django Project**:

    If you don't have a Django project yet, create one by running:

    ```bash
    django-admin startproject your_project
    cd your_project
    ```

3. **Add Static Files**:

    Ensure you have a folder named `static` in your project where you store your CSS, JavaScript, and image files. Place the images you wish to use in the `static/images` folder.

4. **Create HTML Template**:

    Place the provided HTML code in a template file, e.g., `templates/index.html`.

5. **Load Static Files in Django**:

    Make sure to load static files at the top of your HTML template by including:

    ```django
    {% load static %}
    ```

6. **Run the Django Server**:

    To view the page locally, run the Django server:

    ```bash
    python manage.py runserver
    ```

    Navigate to `http://127.0.0.1:8000/` to see the page.

## Code Explanation

- **Navbar**: The navbar is styled using Bootstrap classes and includes a dropdown menu.
- **Carousel**: A Bootstrap carousel is used to display images (`pexels1.jpg`, `pexels2.jpg`, and `pexels3.jpg`). These images are loaded using Django's `{% static %}` template tag.
- **ScrollSpy**: The ScrollSpy feature highlights navigation links as you scroll through the corresponding sections on the page.

## Customization

- Replace the image paths in the carousel with your own images in the `static/images` folder.
- Modify the content in the `<h4>` and `<p>` tags inside the `scrollspy-example` div to fit your needs.
- You can further customize the Bootstrap styles by modifying the `navbar`, `carousel`, or `scrollspy` sections as needed.
