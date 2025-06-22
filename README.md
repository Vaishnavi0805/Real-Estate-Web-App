# 🏡 Real Estate Price Predictor

A web application that predicts New York real estate prices using a Linear Regression model trained on live data scraped from Trulia. The app includes user registration, login functionality, and an easy-to-use prediction form.

---

## 📦 Features

- 🔐 User registration and login system with MySQL
- 🧠 Predicts property prices using a trained Linear Regression model
- 🕷️ Scrapes real estate listings from Trulia using Selenium
- 🏙️ Uses features like location, area, beds, baths, and year built
- 🖥️ Clean interface built with Flask and Jinja templates

---

## 📊 Tech Stack

- **Frontend**: HTML, CSS (Jinja Templates)
- **Backend**: Python, Flask
- **ML Model**: Linear Regression (Scikit-learn)
- **Database**: MySQL (Flask-MySQLdb)
- **Scraping**: Selenium, BeautifulSoup

---

## 🤖 How It Works

1. **Data Collection**:  
   - Selenium-based scraper navigates Trulia listings
   - Extracts fields like price, city, bed/bath count, AC, area, etc.
   - Stores data in `Trulia_Real_Estate.csv`

2. **Model Training**:  
   - Data is preprocessed and used to train a Linear Regression model
   - Model is serialized with `pickle`

3. **Flask App**:  
   - Users register/login
   - Enter property features in form
   - Model predicts price and displays result

---

## 🚀 Getting Started

### 🔧 Prerequisites

- Python 3.9+
- ChromeDriver installed
- MySQL with `flaskdb` database and `accounts` table created

### 💾 Installation

```bash
git clone https://github.com/yourusername/real-estate-price-predictor.git
cd real-estate-price-predictor
pip install -r requirements.txt
python app.py
```

Go to http://localhost:5000 in your browser.



