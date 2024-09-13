# Flask App Development Guide

## General instructions
- Write clean, idiomatic Python code. Prefer functions over classes. Try to keep functions short and easily readable, follow the Zen of Python here. 
- Don't overcomplicate things, prefer simplicity over complexity. It is really important that your code is readable even by a Junior Python Developer.
- Always use the follwing stack: Flask, Flask-Login, Flask-SQLAlchemy, Flask-Migrate and Flask-WTF. Create a requirements.txt without pinned versions.
- In the base template (base.html) link Tailwind CSS and jQuery. Use Poppins by Google as a font. For icons, use Font-Awesome.
- Use SQLite for the database (app.db)
- If you require a third party dependency not mentioned above, always prefer a simple Python implementation over including another library for just one function.
- The app (app.py) should run at port 3000 with reload (reload the app if a template changes)
- Use Google-style docstrings
- Use type hints where possible (PEP 484)
- If you implement user authentication (if the app requires it), do it in a secure way (eg. strong passwords requirements). It should be clear for the user how to register and how to login. Default expiration for user auth cookie should be 1 year and users should be remembered by default (but the user should be given the option to not be remembered). User auth is always based on username and password (not email).

## Styling and look-and-feel
- Strictly minimalistic, black and white design. Use accent colors sparingly, only for critical user interactions or important information. For accent colors, only use purple.
- Utilize negative space effectively to create a clean, uncluttered interface.
- Employ a flat design aesthetic, avoiding shadows, gradients, or complex textures.
- Use Poppins font (by Google) for all text to maintain a consistent, modern look.
- Prefer icons over text where possible, using Font-Awesome for a cohesive icon set.
- Emojis can be used sparingly to add a touch of personality where appropriate.
- Aim for high contrast ratios to ensure readability and accessibility.
- Implement subtle hover effects on interactive elements to improve user feedback.
- Use thin, elegant lines for separators or borders when necessary.
- Keep UI elements to a minimum, focusing on essential functionality and content.

## Development environment information
- The Flask app runs in a virtual environment (./venv) on Ubuntu 24 LTS and Python 3.12.
- Environment variables need to be loaded from a .env file with python-dotenv

# Special remarks
- Always implement a REST(like) JSON API for the important actions/methods. Users should get an API access key (which they can reset by clicking a button).
- Include a page with API documentation (which is publicly accessible)
- Implement OpenAPI spec for the full API you implement.

# Lessons learned during development
During development, add lessons learned here based on feedback by the user:
- Don't use external libraries that are under non-permissive licenses or copyleft licenses
