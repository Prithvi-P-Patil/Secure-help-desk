## Day 1 – Monday 23 November 2026

### What I did
- installed Vs code and python and Flask app on GitHub

### Problems I faced and how I fixed them
- port 5000 taken by airplay, used 5001
Copilot off · .DS_Store ignored · "Don't Allow" local network · debug mode only for local development · token instead of password
### Security decisions I made (and why)
-

### What I learned
- I ran pip freeze > requirements.txt, pip looked inside the venv and wrote down everything installed: Flask, plus the libraries Flask depends on (Werkzeug, Jinja2, Click and others), each with a version number like flask==3.1.3.

Why it matters:

the venv folder is not uploaded to GitHub (it's in .gitignore), so anyone downloading the project has no libraries.
They create their own venv and run pip install -r requirements.txt. pip reads the list and installs the exact same versions you used.

- 200 means "OK, success": the server found the page and sent it back.

## Day 2 - Wednesday 25 November 2026