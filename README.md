# ☁️ CloudCost

A simple web application for **estimating AWS cloud service costs** based on infrastructure and usage requirements.

CloudCost is designed to make cloud cost estimation easier for developers and technical teams by providing a clean interface for exploring AWS service costs and understanding expected monthly expenses.

## ✨ Features

* 📊 AWS service cost estimation
* ⚡ Simple and responsive landing page
* 🧩 Step-by-step cost estimation workflow
* 🖥️ Dashboard interface
* 🎨 Clean, minimal UI
* 🌐 Flask-based web application

## 🛠️ Tech Stack

* **Backend:** Python, Flask
* **Frontend:** HTML, CSS
* **Templating:** Jinja2
* **Deployment:** Render

## 📁 Project Structure

```text
awscost/
│
├── app.py
│
├── templates/
│   ├── home.html
│   ├── navbar.html
│   └── footer.html
│
└── static/
    ├── css/
    │   ├── style.css
    │   └── components.css
    │
    └── img/
        ├── hero_img.png
        └── navicon.png
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd awscost
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**macOS/Linux**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install flask gunicorn
```

### 4. Run the application

```bash
python app.py
```

The application will be available at:

```text
http://127.0.0.1:5000
```

## ☁️ Deployment on Render

Create a **Web Service** on Render and use:

**Build Command**

```bash
pip install -r requirements.txt
```

**Start Command**

```bash
gunicorn app:app
```

If you don't have a `requirements.txt` file yet, create one containing:

```text
Flask
gunicorn
```

You can also generate it locally with:

```bash
pip freeze > requirements.txt
```

## 📌 Current Status

CloudCost currently provides the core Flask application structure and landing page. The dashboard and AWS cost-estimation functionality can be extended as the project develops.

## 📄 License

This project is developed for educational and project purposes.
