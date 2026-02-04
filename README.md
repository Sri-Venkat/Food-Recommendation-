🍽️ Food Recommendation System
Flask-Based Rule-Based Web Application
📌 Project Overview

The Food Recommendation System is a Flask-based web application that provides users with food suggestions, traditional recipes, and restaurant browsing through a rule-based chatbot and dynamic web interface.

Instead of using Machine Learning or Artificial Intelligence models, this system operates on deterministic logic, where predefined user queries are matched with structured responses. The application demonstrates backend routing, frontend template rendering, and interactive user engagement using Python and Flask.

🎯 Objectives

Develop a full-stack food recommendation platform using Flask

Implement a rule-based chatbot for user interaction

Provide dynamic restaurant and menu browsing

Enable autocomplete suggestions for faster user input

Demonstrate real-world web application architecture

🛠️ Technologies Used
Backend

Python 3

Flask – Lightweight web framework for routing and backend logic

Frontend

HTML5

CSS3

Jinja2 Templates – Dynamic content rendering

Tools & Platforms

VS Code – Development environment

Git & GitHub – Version control and hosting

🧠 System Architecture
User → Browser → Flask Server → Rule Engine → Templates → Response → User

Architecture Explanation

The user interacts with the web interface through a browser

Requests are sent to the Flask backend via routes

The rule engine checks user input against predefined responses

Flask renders the appropriate HTML templates

The final output is displayed to the user

⚙️ Key Features

Rule-based chatbot for food-related queries

Autocomplete system for guided user input

Traditional food and recipe navigation pages

Dynamic restaurant listing and menu display

Clean and user-friendly web interface

Lightweight and fast backend performance

📂 Project Structure
Food-Recommendation/
│
├── app.py
├── templates/
│   ├── index.html
│   ├── welcome.html
│   ├── restaurants.html
│   ├── restaurant_menu.html
│   ├── MysoreMasalaDosa.html
│   ├── KharaPongal.html
│   ├── NeerDosa.html
│   ├── RagiMude.html
│   └── ...
│
├── static/
│   └── (CSS / Images if added)
│
├── .gitignore
└── README.md

▶️ How to Run the Project
1️⃣ Install Dependencies

Make sure Python is installed, then install Flask:

pip install flask

2️⃣ Run the Application
python app.py

3️⃣ Open in Browser

Visit:

http://127.0.0.1:5000

🔍 Core Logic Explanation
Rule-Based Chatbot System

The chatbot uses exact string matching to respond to user queries. Each user input is compared against a predefined dictionary of responses.

def get_bot_response(user_input):
    for key, value in responses.items():
        if user_input == key:
            return value


This ensures predictable and fast responses without requiring training data or machine learning models.

Autocomplete Suggestion Engine

As users type, the system suggests relevant queries using substring matching:

def get_autocomplete_suggestions(query):
    return [s for s in suggestions if query in s]


This improves usability and reduces typing effort.

Restaurant & Menu Rendering

Restaurant data is stored in a structured Python list and passed dynamically to HTML templates using Flask’s rendering engine:

@app.route('/restaurants')
def list_restaurants():
    return render_template('restaurants.html', restaurants=restaurants)

📈 Future Enhancements

Convert rule-based chatbot to an NLP-based AI chatbot

Add Machine Learning recommendation engine

User authentication and profile system

Database integration (MySQL / MongoDB)

Admin dashboard for managing restaurants and menus

Cloud deployment (Render / Railway / AWS)

🎓 Academic Relevance

This project demonstrates:

Full-stack web application development

Backend routing and API handling

Rule-based system design

Template rendering using Jinja2

Scalable architecture planning

👨‍💻 Author

Venkat V
Information Science & Engineering
GitHub: https://github.com/Sri-Venkat
