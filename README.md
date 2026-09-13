
# Xvera Labs

Xvera Labs is a Django-based corporate website designed for a technology and consulting company. The project includes the main landing page, about section, services, projects, blogs, contact page, FAQ pages, and a modular app structure for future expansion.

## Features

- Home page and marketing landing page
- About Us section with company, culture, diversity, and career pages
- Service pages for consulting and advanced technology offerings
- Project and portfolio showcase pages
- Blog and case study pages
- FAQ, privacy policy, and terms pages
- Contact us page
- User authentication pages for sign in and sign up
- Django admin for content management
- Responsive template-based frontend with static media support

## Tech Stack

- Python 3.10+
- Django 6.0.6
- Django REST Framework
- SQLite (development database)
- Pillow for image handling
- HTML, CSS, and JavaScript templates

## Project Structure

```bash
xveralabs/
├── apps/
│   ├── about_us/
│   ├── blogs/
│   ├── contact/
│   ├── main/
│   ├── portfolio/
│   ├── projects/
│   ├── services/
│   ├── team/
│   ├── utils/
│   └── __init__.py
├── core/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── media/
├── static/
├── templates/
├── db.sqlite3
├── manage.py
├── requirements.txt
├── README.md
└── .gitignore
```

## Apps Overview

- apps.main: homepage and primary public pages
- apps.about_us: company history, culture, diversity, and team-related pages
- apps.services: consulting and technology service categories
- apps.projects: project or portfolio-related app structure
- apps.portfolio: portfolio data and views
- apps.contact: contact-related app
- apps.blogs: blog content area
- apps.utils: shared utility app
- apps.team: team-specific logic and models

## Key Routes

The project includes routes such as:

- /
- /about-us/company/
- /about-us/why-choose-us/
- /contact-us/
- /services/
- /projects/
- /blogs/
- /case-studies/
- /faqs/
- /terms-conditions/
- /privacy-policy/
- /signin/
- /signup/
- /sqa/
- /web-development/
- /product-development/
- /dev-ops/
- /staff-augmentation/

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/MuhammadNouman769/xveralabs.git

cd  xveralabs
```

### 2. Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Apply database migrations

```bash
python manage.py migrate
```

### 5. Create a superuser

```bash
python manage.py createsuperuser
```

### 6. Run the development server

```bash
python manage.py runserver
```

Then open:

```text
http://127.0.0.1:8000/
```

## Admin Access

After creating the superuser, you can access Django admin here:

```text
http://127.0.0.1:8000/admin/
```

## Configuration Notes

- The project currently uses SQLite for local development.
- DEBUG is enabled in settings for local development.
- For production, update the following before deployment:
  - SECRET_KEY
  - DEBUG
  - ALLOWED_HOSTS
  - database configuration
  - static/media deployment settings

## Notes

This project is a template-based Django website for a business/agency brand and is suitable for extension into a production-ready company website with CMS integration, contact form processing, and deployment optimization.

## License

This project currently does not include a formal license file. If you are publishing or sharing it publicly, add a license according to your project requirements.
