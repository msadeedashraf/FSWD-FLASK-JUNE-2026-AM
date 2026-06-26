# FSWD-FLASK-JUNE-2026-AM
## What is Flask?

-  Flask is a lightweight WSGI web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications.

**Flask** and **Django** are both popular Python web frameworks, but they follow different philosophies.

| Feature           | Flask                                  | Django                                                  |
| ----------------- | -------------------------------------- | ------------------------------------------------------- |
| Philosophy        | Minimalist ("micro-framework")         | Batteries-included                                      |
| Learning Curve    | Easier to start                        | Steeper, more features to learn                         |
| Project Size      | Small to medium applications, APIs     | Medium to large applications                            |
| Flexibility       | Highly flexible; choose your own tools | More opinionated; follows conventions                   |
| Built-in Features | Very few                               | ORM, authentication, admin panel, forms, sessions, etc. |
| Database Support  | Requires extensions for ORM            | Built-in ORM                                            |
| Admin Interface   | Not included                           | Built-in admin dashboard                                |
| Performance       | Lightweight and fast for simple apps   | Slightly heavier but scalable                           |
| Customization     | High                                   | Moderate                                                |
| Best For          | APIs, microservices, prototypes        | Full-featured web applications                          |

### Flask Example

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello, World!"

if __name__ == "__main__":
    app.run()
```

### Django Example

```python
from django.http import HttpResponse

def home(request):
    return HttpResponse("Hello, World!")
```

### When to Choose Flask

* Building REST APIs
* Creating small applications
* Learning web development
* Needing complete control over architecture
* Rapid prototyping

### When to Choose Django

* Building large web applications
* Requiring authentication and user management
* Needing an admin dashboard
* Working with relational databases extensively
* Wanting a structured, scalable framework

### Simple Analogy

* **Flask** is like buying individual ingredients and cooking exactly what you want.
* **Django** is like getting a complete kitchen setup with appliances, utensils, and recipes included.

**Recommendation:** If you're a beginner learning Python web development, start with Flask to understand web fundamentals. If you're building a production-ready application with authentication, database models, and admin functionality, Django can save significant development time.

## Big Picture
![Big Picture](/Assets/big-picture.png)


## Flask Quick start
[Flask](https://flask.palletsprojects.com/en/stable/quickstart/)

## Create Environtment

![](/Assets/flask-hello-world-0.png)

```
mkdir hello-world
cd hello-world
py -3 -m venv my-flask-env
```

```
.\my-flask-env\Scripts\activate
```

```
pip install Flask
```

![](/Assets/flask-hello-world-1.png)

- create a app.py file in the hello-world folder 

![](/Assets/flask-hello-world-2.png)

```
@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"

if __name__ == "__main__":
    app.run(debug=True)
```

![](/Assets/flask-hello-world-3.png)

```
python app.py
```
- Open the browser and copy the highligted url (http://127.0.0.1:5000/)

![](/Assets/flask-hello-world-4.png.png)
