# Pradyumna's Portfolio

A modern, responsive portfolio website built with Django featuring a sleek dark theme with glassmorphism effects.

## ✨ Features

- **Modern Dark Theme** - Premium aesthetic with purple/blue gradient accents
- **Glassmorphism UI** - Frosted glass effects on navigation and cards
- **Smooth Animations** - Hover effects and micro-interactions
- **Responsive Design** - Works beautifully on all devices
- **Blog System** - Built-in blog with post management
- **Project Showcase** - Display your work with image cards

## 🚀 Quick Start

### Prerequisites

- Python 3.8+
- pip (Python package manager)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/pradyumnakr/portfolio-project.git
   cd portfolio-project
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install django
   ```

4. **Run database migrations**
   ```bash
   python manage.py migrate
   ```

5. **Start the development server**
   ```bash
   python manage.py runserver
   ```

6. **Open your browser**
   
   Visit [http://127.0.0.1:8000](http://127.0.0.1:8000)

## 📁 Project Structure

```
portfolio-project/
├── blog/                   # Blog app
│   ├── templates/blog/     # Blog templates
│   ├── models.py           # Blog post model
│   └── views.py            # Blog views
├── jobs/                   # Projects/Jobs app
│   ├── templates/jobs/     # Home page template
│   ├── models.py           # Job/Project model
│   └── views.py            # Home view
├── portfolio/              # Main project settings
│   ├── static/             # Static files (CSS, images)
│   │   ├── style.css       # Custom styles
│   │   └── pradyumna.png   # Profile image
│   ├── settings.py         # Django settings
│   └── urls.py             # URL routing
└── manage.py               # Django management script
```

## ⚙️ Configuration

### Database

By default, the project uses SQLite. To change the database, edit `portfolio/settings.py`:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    }
}
```

### Static Files

Static files are located in `portfolio/static/`. To customize:

- **Profile Image**: Replace `pradyumna.png` with your own image
- **Resume**: Replace `Internshala_Resume_Guide.pdf` with your resume
- **Styles**: Edit `style.css` to customize colors and design

### Admin Panel

1. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```

2. Access admin at [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin)

3. Add blog posts and projects through the admin interface

## 🎨 Customization

### Changing Colors

Edit CSS variables in `portfolio/static/style.css`:

```css
:root {
  --accent-primary: #6366f1;    /* Primary purple */
  --accent-secondary: #8b5cf6;  /* Secondary purple */
  --bg-primary: #0a0a0f;        /* Background */
}
```

### Updating Personal Info

Edit `jobs/templates/jobs/home.html` to update:
- Name and tagline
- Description text
- Contact email
- Social links

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Pradyumna**
- LinkedIn: [@pradyumnakr](https://www.linkedin.com/in/pradyumnakr/)
- GitHub: [@pradyumnakr](https://github.com/pradyumnakr)
