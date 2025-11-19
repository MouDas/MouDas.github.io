# Meal Planner Project

This project has **two parts**:

1. **Blog (`my-blog`)** – tracks daily progress building the Meal Planner app.  
2. **Web App (`meal-planner-webapp`)** – prototype app for planning weekly meals, generating grocery lists, and providing prep instructions.

---

## Part 1: Blog Setup (`my-blog`)

The blog is built using **GitHub Pages** and **Markdown**. It documents daily progress, setup steps, and project notes.

### Blog Folder Structure

my-blog/
├── _posts/ # Daily posts in Markdown
│ ├── 2025-11-18-first-post.md
│ └── 2025-11-19-setup-dev-environment.md
├── index.md # Homepage listing posts
├── _config.yml # Blog settings
└── README.md # This documentation

sql
Copy code

### How to Add a New Post

1. Go to `_posts/` and create a new Markdown file using the format:
YYYY-MM-DD-title.md

yaml
Copy code
2. Include front matter at the top:

```markdown
---
layout: post
title: "Day X: Your post title"
date: YYYY-MM-DD
---
Write your post content below the front matter.

Commit and push:

bash
Copy code
git add .
git commit -m "Add Day X blog post"
git push
Your post will automatically appear on the homepage:
https://MouDas.github.io

Day-by-Day Progress (Blog)
Day 1: Created blog, added first post, verified GitHub Pages worked

Day 2: Set up second post, added basic folder structure, started documenting setup

Part 2: Meal Planner Web App (meal-planner-webapp)
This is a Flask web app prototype to plan weekly meals and generate grocery lists.

Folder Structure
csharp
Copy code
meal-planner-webapp/
├── app.py            # Main Flask app
├── templates/        # HTML pages
│   └── index.html    # Homepage
├── static/           # CSS or images (optional)
├── recipes.json      # Recipe database (to be added)
├── menu_history.json # Track last 2 weeks' menus (to be added)
└── README.md         # This documentation
Tools & Technologies
Python 3.13

Flask 3.1.2

VS Code

HTML / CSS for frontend

Setup Instructions
Navigate to your project folder:

bash
Copy code
cd ~/meal-planner-webapp
Install Flask (if not already installed):

bash
Copy code
pip3 install flask
Minimal Flask app (app.py):

python
Copy code
from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def home():
    return render_template("index.html")

if __name__ == "__main__":
    app.run(debug=True)
Create homepage templates/index.html:

html
Copy code
<!DOCTYPE html>
<html>
<head>
    <title>Meal Planner App</title>
</head>
<body>
    <h1>Welcome to your Meal Planner!</h1>
    <p>This is your first web app prototype.</p>
</body>
</html>
Run the app locally:

bash
Copy code
python3 app.py
Open your browser at:

arduino
Copy code
http://localhost:5000
If “Access Denied” appears, try http://127.0.0.1:5000 or make sure Flask is allowed through your firewall.

Day-by-Day Progress (Web App)
Installed Python 3 and verified version

Installed Flask 3.1.2

Created project folder structure (templates, static)

Built minimal Flask app with homepage

Verified app runs locally in browser

Next Steps
Add recipes.json to store your recipes

Build menu generator avoiding repeats from last 2 weeks

Generate grocery lists and prep instructions

Parse WhatsApp exported messages for past menus

Optional: deploy online for access on mobile

Notes
Keep blog and web app in separate folders

Use README to track setup, progress, and instructions

Add new features and daily progress under “Day X – Feature” sections

yaml
Copy code

---

This README now:

- Combines **blog setup** and **web app setup**  
- Documents **every step we’ve done today**  
- Leaves space to **add new features / daily progress**  