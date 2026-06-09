# Flask Jinja2 Web App

A beginner-friendly web application built using Flask and Jinja2 templates. This project demonstrates core Flask concepts such as routing, form handling, template rendering, dynamic URLs, and passing data between Python and HTML.

## Features

- Flask routing
- Multiple web pages
- Form submission using POST requests
- Dynamic URL parameters
- Jinja2 template rendering
- Conditional statements in templates
- Loops in templates
- Passing dictionaries from Flask to HTML
- Displaying dynamic results based on user input

## Technologies Used

- Python
- Flask
- HTML5
- Jinja2

## Project Structure

project/
│
├── jinja.py
│
└── templates/
    ├── index.html
    ├── about.html
    ├── form.html
    ├── result.html
    └── result1.html

## Routes

| Route | Description |
|---------|-------------|
| `/` | Welcome page |
| `/index` | Home page |
| `/about` | About page |
| `/submit` | Form submission page |
| `/success/<score>` | Displays pass/fail result |
| `/successres/<score>` | Displays result data in a table |
| `/successif/<score>` | Demonstrates Jinja2 conditional rendering |

## Concepts Demonstrated

### Flask Routing

```python
@app.route("/")
```

Maps URLs to Python functions.

### Form Handling

```python
request.form['name']
```

Retrieves user input submitted through forms.

### Dynamic URLs

```python
@app.route('/success/<int:score>')
```

Accepts values directly from the URL.

Example:

```
http://127.0.0.1:5000/success/75
```

### Jinja2 Variables

```html
{{ results }}
```

Displays dynamic values from Flask.

### Jinja2 Conditionals

```html
{% if results >= 50 %}
```

Used to render different content based on conditions.

### Jinja2 Loops

```html
{% for key, value in results.items() %}
```

Used to iterate through dictionaries and display data dynamically.

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/Flask-Jinja2-Web-App.git
```

### Navigate to Project Folder

```bash
cd Flask-Jinja2-Web-App
```

### Install Flask

```bash
pip install flask
```

### Run the Application

```bash
python jinja.py
```

### Open Browser

```
http://127.0.0.1:5000
```

## Learning Outcomes

Through this project I learned:

- Creating Flask applications
- Defining routes
- Handling GET and POST requests
- Rendering HTML templates
- Passing data from Python to HTML
- Using Jinja2 variables
- Using Jinja2 loops
- Using Jinja2 conditionals
- Working with dynamic URL parameters

## Future Improvements

- Add CSS styling
- Create a navigation bar
- Add user authentication
- Store form data in a database
- Deploy the application online

## Author

Krishna Khajuria
