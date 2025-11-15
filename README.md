# Portfolio website

The project demonstrates Python Flask web framework integration with a ready-made HTML/CSS/Javascript portfolio template. It includes server-side contact form processing, dynamic routing, and modern Python packaging. The Work page is ready to showcase development projects.

🌐 **Live Demo**: [ry4n.pythonanywhere.com](https://ry4n.pythonanywhere.com)

## What this project does

- Flask integration: Converts static HTML template to dynamic Flask application
- Contact form backend: Implements server-side form processing with CSV storage
- Template routing: Sets up proper URL routing for multi-page navigation
- Python packaging: Modern dependency management with uv and pyproject.toml
- Deployment ready: Configured for PythonAnywhere hosting

## Technologies

My implementation:

- Backend: Python 3.10, Flask 3.1.2
- Package management: uv Python project packaging
- Data storage: CSV file handling

Original "Univers" template:

- Frontend: HTML5, CSS3, JavaScript, Bootstrap 3
- Icons: Font Awesome 4.7.0
- Fonts: Google Fonts (Roboto, Roboto Mono)

## Quick start

### Prerequisites

- Python 3.10+
- [uv](https://github.com/astral-sh/uv) package manager

### Installation

1. **Clone the repository**
   ```zsh
   git clone https://github.com/nite-stocker/portfolio.git
   cd portfolio
   ```

2. **Install dependencies**
   ```zash
   uv sync
   ```

3. **Run the application**
   ```zash
   uv run flask run --debug
   ```

4. **Open your browser**
    - Navigate to `http://localhost:5000`

## Project structure

```
portfolio/
├── app.py              # Flask application entry point
├── pyproject.toml      # Modern Python project config
├── static/
│   ├── main.*.css      # Stylesheets
│   ├── main.*.js       # JavaScript bundle
│   └── assets/         # Images and icons
└── templates/          # Jinja2 HTML templates
    ├── index.html      # Home page
    ├── about.html      # About page
    ├── works.html      # Projects showcase
    ├── work.html       # Individual project views
    ├── contact.html    # Contact form
    └── thankyou.html   # Form confirmation
```

## Development

### Flask-specific customizations

New routes:

1. Add route handler in `app.py`
2. Create corresponding Jinja2 template in `templates/`
3. Update navigation links in existing templates

Contact form enhancement:

- Stores submissions in `.csv` file
- Built with Flask's request handling
- Ready for database integration (PostgreSQL, SQLite)
- Consider adding email notifications and validation

Template modification:

- Original static HTML converted to Jinja2 templates
- Flask url_for() integration for asset linking
- Template inheritance could be implemented for Don't Repeat Yourself (DRY) code

## Deployment

The application is designed for easy deployment on platforms like:

- [PythonAnywhere](https://pythonanywhere.com) (current hosting)
- Or any Web Server Gateway Interface (WSGI)-compatible server
    - [Anvil](https://anvil.works)
    - [Fly.io](https://fly.io/docs/python/)
    - [Heroku](https://www.heroku.com/python/)
    - [Railway](https://docs.railway.com/guides/languages-frameworks#python)
    - [Taipy](https://taipy.io)

## Credits

**Original design and frontend:**

- Univers portfolio website template from [free-css.com](https://www.free-css.com/free-css-templates/page270/univers) (website no longer resolves), by [Orson.io](http://orson.io) for [mashup-template.com](http://www.mashup-template.com) with images by [Unsplash](https://www.unsplash.com).

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request