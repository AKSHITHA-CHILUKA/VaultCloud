
# A Cloud Storage of Files

Users are provided with **AES encryption of files** for secure storage and retrieval.  

---

## 🚀 Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/your-username/Secure-Personal-Cloud.git
cd Secure-Personal-Cloud
```

### 2. Create a virtual environment
```bash
python -m venv venv
```
Activate it:

**Windows (PowerShell):**
```bash
venv\Scripts\activate
```
**Linux / MacOS:**
```bash
source venv/bin/activate
```

### 3. Install dependencies
All required packages are listed in requirements.txt. Install them with:
```bash
pip install -r requirements.txt
```

---

## 🖥️ Instructions for Web Client
Run these commands inside the project directory:
```bash
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```
Now open your browser and go to:
👉 http://127.0.0.1:8000

---

## 🐧 Instructions for Linux Client
Install dependencies:
```bash
pip install django-database-storage tabulate
```
Add spc executable to PATH:
The bash executable spc is found inside:
```bash
Secure-Personal-Cloud/bin/
```
Add it to your environment PATH variable. Example:
```bash
export PATH=$PATH:/path/to/Secure-Personal-Cloud/bin
```
Run the client:
```bash
spc help
```

---

## 🪟 Instructions for Windows Client
Make sure the virtual environment is activated (`venv\Scripts\activate`).

Install the same dependencies:
```bash
pip install django-database-storage tabulate
```
To run the client script on Windows, you can directly execute it using Python:
```bash
python bin\spc help
```
(Or add the `bin\` folder to your system PATH for easier access.)

---

## ✅ Notes
- Default database is SQLite (configured in `settings.py`).
- For production, configure PostgreSQL or another supported database.
- Static files are served from the `static/` directory.
- Make sure to apply migrations before running the server.

---

