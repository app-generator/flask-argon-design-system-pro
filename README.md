# [Flask Argon System PRO](https://appseed.us/product/argon-design-system-pro/flask/)

Seed project generated by AppSeed in **Flask** Framework on top of **Argon Design System PRO** with database, authentication, helpers and Docker support. Argon Design System PRO is built with over 1100 individual elements, 43 sections and 17 example pages giving you the freedom of choosing and combining. 

- 👉 [Flask Argon System PRO](https://appseed.us/product/argon-design-system-pro/flask/) - product page
- 👉 [Flask Argon System PRO](https://flask-argon-design-system-pro.appseed-srv1.com/) - LIVE App
- 👉 [Complete documentation](https://docs.appseed.us/boilerplate-code/boilerplate-flask) - `Learn how to use and update the product`
  
<br />

> Features

- `Up-to-date dependencies`
- Database: `mysql`
- `DB Tools`: SQLAlchemy ORM, Flask-Migrate (schema migrations)
- Session-Based authentication (via **flask_login**), Forms validation

<br />

![Argon Design PRO - Seed project crafted by AppSeed.](https://user-images.githubusercontent.com/51070104/187922792-7f7c8bb9-25a5-4129-a0fe-6bbfba82501d.png)

<br />

## ✨ Start the app in Docker

> **Step 1** - Download the [code](https://appseed.us/product/argon-design-system-pro/flask/) and unzip the sources (requires a `purchase`). 

```bash
$ # Get the code
$ unzip flask-argon-design-system-pro.zip
$ cd flask-argon-design-system-pro
```

<br />

> **Step 2** - Start the APP in `Docker`

```bash
$ docker-compose up --build 
```

Visit `http://localhost:5085` in your browser. The app should be up & running.

<br />


## ✨ How to use it

> Download the [code](https://appseed.us/product/argon-design-system-pro/flask/) and unzip the sources (requires a `purchase`). 

```bash
$ # Get the code
$ unzip flask-argon-design-system-pro.zip
$ cd flask-argon-design-system-pro
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Flask Environment

```bash
$ export FLASK_APP=run.py
$ export FLASK_ENV=development
```

<br />

> Start the app

```bash
$ flask run
```

At this point, the app runs at `http://127.0.0.1:5000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Flask Environment

```bash
$ # CMD 
$ set FLASK_APP=run.py
$ set FLASK_ENV=development
$
$ # Powershell
$ $env:FLASK_APP = ".\run.py"
$ $env:FLASK_ENV = "development"
```

<br />

> Start the app

```bash
$ flask run
```

At this point, the app runs at `http://127.0.0.1:5000/`. 

<br />

### 👉 Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app via `flask run`
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:5000/register`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:5000/login`

<br />

## ✨ Code-base structure

The project is coded using blueprints, app factory pattern, dual configuration profile (development and production) and an intuitive structure presented bellow:

```bash
< PROJECT ROOT >
   |
   |-- apps/
   |    |
   |    |-- home/                           # A simple app that serve HTML files
   |    |    |-- routes.py                  # Define app routes
   |    |
   |    |-- authentication/                 # Handles auth routes (login and register)
   |    |    |-- routes.py                  # Define authentication routes  
   |    |    |-- models.py                  # Defines models  
   |    |    |-- forms.py                   # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>          # CSS files, Javascripts files
   |    |
   |    |-- templates/                      # Templates used to render pages
   |    |    |-- includes/                  # HTML chunks and components
   |    |    |    |-- navigation.html       # Top menu component
   |    |    |    |-- sidebar.html          # Sidebar component
   |    |    |    |-- footer.html           # App Footer
   |    |    |    |-- scripts.html          # Scripts common to all pages
   |    |    |
   |    |    |-- layouts/                   # Master pages
   |    |    |    |-- base.html             # Used by common pages
   |    |    |
   |    |    |-- accounts/                  # Authentication pages
   |    |    |    |-- login.html            # Login page
   |    |    |    |-- register.html         # Register page
   |    |    |
   |    |    |-- home/                      # UI Kit Pages
   |    |         |-- index.html            # Index page
   |    |         |-- page-404.html         # 404 page
   |    |         |-- *.html                # All other pages
   |    |    
   |  config.py                             # Set up the app
   |    __init__.py                         # Initialize the app
   |
   |-- requirements.txt                     # App Dependencies
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- run.py                               # Start the app - WSGI gateway
   |
   |-- ************************************************************************
```

<br />

---
 [Flask Argon System PRO](https://appseed.us/product/argon-design-system-pro/flask/) - Seed project generated by **[AppSeed Generator](https://appseed.us/generator/)**.
