# Content Craft - Django Blog Application

## Overview
Content Craft is a Django-based blog application that allows users to create, read, update, and delete blog posts. It includes user authentication, profile management, and a modern, responsive design with Bootstrap and custom CSS. The application supports pagination, user-specific post filtering, and image uploads for user profiles.

## Features
- **User Authentication**: Register, login, logout, and password reset functionality.
- **Blog Posts**: Create, view, update, and delete posts with a rich text editor.
- **User Profiles**: Update username, email, and profile picture with automatic image resizing.
- **Responsive Design**: Modern UI with Bootstrap 4, custom CSS, and a sticky header.
- **Pagination**: Posts are paginated (5 per page) for better performance.
- **Social Features**: View posts by specific users and follow links to social media.

## Project Structure
```
django_project/
├── blog/
│   ├── migrations/
│   ├── templates/blog/
│   │   ├── base.html
│   │   ├── home.html
│   │   ├── about.html
│   │   ├── post_detail.html
│   │   ├── post_form.html
│   │   ├── post_delete.html
│   │   └── user_posts.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   ├── views.py
│   └── static/blog/
│       ├── main.css
│       ├── logo.jpg
├── users/
│   ├── migrations/
│   ├── templates/users/
│   │   ├── login.html
│   │   ├── logout.html
│   │   ├── profile.html
│   │   ├── register.html
│   │   ├── password_reset.html
│   │   ├── password_reset_done.html
│   │   ├── password_reset_confirm.html
│   │   └── password_reset_complete.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── signals.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── django_project/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
├── media/
│   ├── profile_pics/
│   └── default.jpg
├── db.sqlite3
├── manage.py
└── README.md
```

## Requirements
- Python 3.6+
- Django 2.1
- Pillow (for image processing)
- crispy-bootstrap4 (for form styling)

## Installation
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd django_project
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install django==2.1 pillow crispy-bootstrap4
   ```

4. **Set Up Environment Variables**:
   Create a `.env` file in the project root or set the following environment variables for email functionality:
   ```bash
   export EMAIL_USER='your-email@gmail.com'
   export EMAIL_PASS='your-email-password'
   ```

5. **Run Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Create a Superuser** (optional):
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the Development Server**:
   ```bash
   python manage.py runserver
   ```
   Access the application at `http://127.0.0.1:8000`.

## Usage
- **Home Page**: View all posts with pagination.
- **User Posts**: Filter posts by a specific user via `/user/<username>`.
- **Create Post**: Authenticated users can create posts at `/post/new/`.
- **Update/Delete Post**: Authors can edit or delete their posts via the post detail page.
- **Profile Management**: Update profile details and upload a profile picture at `/profile/`.
- **About Page**: Static page with information about the blog.
- **Admin Panel**: Access at `/admin/` with superuser credentials to manage users and posts.

## Configuration
- **Settings**: Update `django_project/settings.py` for production (e.g., set `DEBUG = False`, configure `ALLOWED_HOSTS`, and use a production-ready database).
- **Static Files**: Run `python manage.py collectstatic` for production.
- **Media Files**: Ensure the `media/` directory is writable for profile picture uploads.
- **Email**: Configure `EMAIL_HOST_USER` and `EMAIL_HOST_PASSWORD` for password reset emails.

## Styling
- **Bootstrap 4**: Used for responsive layouts and components.
- **Custom CSS**: `blog/static/blog/main.css` includes a modern design system with gradients, shadows, and animations.
- **Fonts**: Uses Inter font via system fonts for better performance.
- **Dark Mode**: Automatically adapts to the user's system preferences.

## Contributing
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact
For support or inquiries, contact:
- Email: info@contentcraft.com
- Phone: +1 555-555-5555
- Address: 123 Content Lane, BlogCity, BC 10101

Follow us on social media:
- [Facebook](#)
- [Twitter](#)
- [Instagram](#)
- [LinkedIn](#)

© 2024 Content Craft. All Rights Reserved. Designed by Saim.