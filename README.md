# 🌦️ Weather Application - Django Project

A simple Django-based web app that displays **real-time weather information** for any city using a weather API. It’s perfect for beginners exploring Django and API integration.

---

## 📌 Features

* 🔍 Search weather by city name
* 🌡️ Shows temperature, humidity, pressure, and weather condition
* 🌐 Uses OpenWeatherMap API (or similar)
* 🧱 Built using Python, Django, HTML, and CSS

---

## 🧱 Project Structure

```
weatherapp-master/
├── Scripts/                    # Virtual environment scripts
│   ├── activate, deactivate, pip, python, etc.
├── weatherapplication/         # Main Django project
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── weatherupdates/             # App with logic and templates
│   ├── views.py
│   ├── templates/
│   └── static/
├── manage.py
├── .gitignore
├── pyvenv.cfg
└── README.md
```

---

## ⚙️ How to Run the Project (Locally)

### ✅ Prerequisites

* Python 3.8 or above
* pip
* Virtual environment (`venv`)

### 🧪 Steps to Run

1. **Activate Virtual Environment**
   In terminal or command prompt:

   ```bash
   # PowerShell
   .\Scripts\Activate.ps1

   # Or Command Prompt
   Scripts\activate.bat
   ```

2. **Install Required Packages**
   If you haven’t yet created a `requirements.txt`, run:

   ```bash
   pip install django requests
   ```

   Or if you have `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run Server**

   ```bash
   python manage.py runserver
   ```

4. **View in Browser**
   Open `http://127.0.0.1:8000/`

---

## 🔑 Weather API Setup

1. Get an API key from [OpenWeatherMap](https://openweathermap.org/api)

2. In your `views.py`, use the API key like:

   ```python
   API_KEY = 'your_api_key'
   ```

3. Use it in the request URL:

   ```python
   url = f'https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY}'
   ```

---

## 🧪 Sample Output

**Input:**
`City: Hyderabad`

**Output:**

* Temperature: `30°C`
* Weather: `Clear`
* Humidity: `55%`

---

## 🔮 Future Enhancements

* 🗺️ Country-based search
* 📅 5-day weather forecast
* 🖼️ Weather icons
* 🌐 Add search history or favorite cities
