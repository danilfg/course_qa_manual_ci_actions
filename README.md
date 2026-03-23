Ок, делаю тебе **README уровня топ GitHub проекта** 🚀
(с бейджами, структурой, CI/CD описанием, архитектурой)

---

# 🚀 QA Automation CI/CD Project

### GitHub Actions + PythonAnywhere + OpenWeather API

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![Django](https://img.shields.io/badge/django-4.x-green.svg)
![CI](https://img.shields.io/badge/CI-GitHub_Actions-success)
![Deployment](https://img.shields.io/badge/deploy-PythonAnywhere-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

---

## 📌 Overview

This project demonstrates a **real-world CI/CD pipeline** for a Python web application.

It includes:

* 🌐 Weather API integration (OpenWeatherMap)
* 🔁 Automated deployment via GitHub Actions
* ☁️ Hosting on PythonAnywhere
* 🧪 QA-oriented structure (ready for automation testing)

---

## 🏗️ Architecture

```text
Developer → GitHub → GitHub Actions → PythonAnywhere → Web App
```

### Flow:

1. Developer pushes code to GitHub
2. GitHub Actions workflow is triggered
3. CI pipeline deploys the project to PythonAnywhere
4. Application becomes доступно via web URL

---

## ⚙️ Tech Stack

* Python 3.9+
* Django
* GitHub Actions
* PythonAnywhere
* OpenWeatherMap API

---

## 🚀 Quick Start

### 1. Fork the Repository

```bash
git clone https://github.com/YOUR_USERNAME/course_qa_manual_ci_actions.git
cd course_qa_manual_ci_actions
```

---

### 2. Get OpenWeather API Key

* [https://openweathermap.org](https://openweathermap.org)
* Generate API key

---

### 3. Configure API Key

```python
# weather/views.py
API_KEY = "YOUR_API_KEY"
```

---

### 4. Run Locally

```bash
python manage.py runserver
```

---

## 🔐 Environment Variables (GitHub Secrets)

Go to:

```text
Settings → Secrets and variables → Actions
```

Add:

| Variable                 | Description   |
| ------------------------ | ------------- |
| PYTHONANYWHERE_API_TOKEN | API token     |
| PYTHONANYWHERE_USERNAME  | Your username |
| CONSOLE_ID               | Console ID    |

---

## ⚙️ CI/CD Pipeline

### GitHub Actions Workflow

Triggered on:

```yaml
on:
  push:
    branches: [ main ]
```

### What happens:

* ✅ Code checkout
* ✅ Deployment script execution
* ✅ Project sync with PythonAnywhere

---

## ☁️ Deployment (PythonAnywhere)

### Steps:

1. Create account → [https://pythonanywhere.com](https://pythonanywhere.com)
2. Create Web App
3. Create API Token
4. Create Bash console
5. Copy Console ID

---

## 🌧️ Feature: Humidity

### Backend

```python
weather_info = {
    'humidity': data['main']['humidity'],
}
```

### Frontend

```javascript
<p>Humidity: ${data.humidity}%</p>
```

---

## 📁 Project Structure

```text
project/
│
├── weather/
│   ├── views.py
│   ├── models.py
│
├── templates/
│   └── index.html
│
├── .github/
│   └── workflows/
│       └── deploy.yml
│
├── manage.py
└── requirements.txt
```

---

## 🧪 QA Focus

This project is designed for:

* API testing practice
* CI/CD pipeline understanding
* Automation engineer training

---

## ⚠️ Security Notes

❗ Do NOT store API keys in code
✔ Use GitHub Secrets
✔ Use `.env` in real projects

---

## 📈 Future Improvements

* [ ] Add Pytest tests
* [ ] Add Docker support
* [ ] Add staging environment
* [ ] Add logging (ELK / Grafana)

---

## 👨‍💻 Author

Daniil Nikolaev
QA Automation Engineer | Mentor

---

## ⭐ Support

If you like this project:

👉 Star the repo
👉 Share with others

---

Если хочешь — дальше могу сделать 🔥:

* CI YAML под твой проект (готовый deploy.yml)
* Docker + CI/CD версия (уровень middle+)
* Версию под O-1 (как кейс в портфолио)
