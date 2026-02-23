📘 Python | Web API & Flask Assignment
📌 Overview

This project covers fundamental backend development concepts using Python and Flask, along with important Web API principles.

It includes:

Python OOP Concepts (Polymorphism & Encapsulation)

Web API Fundamentals

REST & SOAP

HTTP Methods

Authentication & Authorization

Flask Framework Basics

🐍 Python OOP Concepts
🔹 Polymorphism

Polymorphism allows the same method name to behave differently depending on the object.

Example:
class Dog:
    def sound(self):
        return "Bark"

class Cat:
    def sound(self):
        return "Meow"

animals = [Dog(), Cat()]

for animal in animals:
    print(animal.sound())
🔹 Encapsulation

Encapsulation means restricting direct access to data and controlling it through methods.

Example:
class Student:
    def __init__(self, name):
        self.__name = name

    def get_name(self):
        return self.__name

student = Student("Rahul")
print(student.get_name())
🌐 Web API Concepts
✅ What is a Web API?

A Web API allows communication between a client and server using HTTP protocol.

✅ REST vs SOAP
REST	SOAP
Architectural style	Protocol
Uses JSON/XML	Uses XML only
Lightweight	Heavy but secure
✅ JSON

JSON (JavaScript Object Notation) is a lightweight format used for data exchange in APIs.

Example:

{
  "name": "Student",
  "age": 20
}
✅ HTTP Methods

GET – Retrieve data

POST – Create data

PUT – Update data

DELETE – Delete data

✅ Authentication & Authorization

Authentication → Verify identity

Authorization → Grant permissions

Common methods:

API Keys

JWT

OAuth

✅ Statelessness in REST

REST APIs are stateless.
Each request contains complete information.
Server does not store client session data.

✅ Common HTTP Status Codes

200 – OK

201 – Created

400 – Bad Request

401 – Unauthorized

404 – Not Found

500 – Internal Server Error

🐍 Flask Framework
✅ What is Flask?

Flask is a lightweight Python web framework used to build web applications and APIs.

✅ Installation
pip install flask
✅ Basic Flask App Structure
flask_project/
│
├── app.py
├── templates/
├── static/
└── requirements.txt
✅ Simple Flask Example
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello World"

if __name__ == "__main__":
    app.run(debug=True)
✅ Routing in Flask

Routing connects URLs to functions using the @app.route() decorator.

✅ Flask Templates

Flask uses Jinja2 template engine to render dynamic HTML pages using render_template().

📚 Topics Covered

Python OOP

Polymorphism

Encapsulation

Web API

REST & SOAP

JSON

HTTP Methods

Authentication & Authorization

API Versioning

Error Handling

Flask

Routing & Templates

🚀 Conclusion

This assignment provides a strong foundation in:

Python programming

Web API architecture

RESTful services

Flask web development
