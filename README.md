# Content Craft Blog

A full-featured blog application built using Django and Bootstrap. This project allows users to register, create posts, view other users' posts, and manage their profiles.

## Features

- User authentication (Login, Register, Logout)
- Profile management with image upload
- Create, read, update, and delete blog posts
- Pagination support
- Responsive design using Bootstrap 4
- Sidebar with additional discovery content
- Newsletter subscription form (non-functional placeholder)
- Footer with contact and social media links

## Technologies Used

- Python 3
- Django
- HTML5 & CSS3
- Bootstrap 4
- JavaScript
- FontAwesome for icons

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/content-craft.git
cd content-craft
```

2. Set up a virtual environment and activate it:

```bash
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Apply migrations and run the server:

```bash
python manage.py migrate
python manage.py runserver
```

5. Visit the blog at `http://127.0.0.1:8000/`

## Directory Structure

- `blog/` - Main app with views, models, templates, and static files
- `users/` - User registration and profile management
- `templates/` - Contains base and page-specific HTML templates
- `static/` - CSS, images, and JavaScript

## License

This project is licensed under the MIT License.

## Author

Created by Muhammad Saim. Reach out on [LinkedIn](https://www.linkedin.com/) or GitHub.
