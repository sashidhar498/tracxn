
# Simple Flask App

This is a **simple Flask application** for user registration and email verification using **AWS SES**.  
Users are allowed to log in **only after verifying their registered email address**.

---

## 📁 Project Structure

```

tracxn/                                 # Root folder
├── instance/                           # Created automatically when DB is initialized
│   └── users.db                        # SQLite database for users
├── myenv/                              # Virtual environment
├── templates/                          # HTML templates
│   └── signup.html                     # User signup page (basic UI)
├── app.py                              # Main Flask application
├── requirements.txt                    # Python dependencies
└── README.md                           # Project documentation

````

---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.x
- SQLite (comes bundled with Python)
- AWS SES account (configured and verified)

---

### Step 1: Create Virtual Environment
```bash
python3 -m venv myenv
````

### Step 2: Activate Virtual Environment

**Windows**

```bash
myenv\Scripts\activate
```

**Linux / macOS**

```bash
source myenv/bin/activate
```

---

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

---

### Step 4: Configure AWS SES

* Verify sender email/domain in AWS SES
* Add AWS credentials and SES configuration in `app.py` (or environment variables)

---

## 🚀 Features

* User registration
* Email verification using AWS SES
* Login allowed only after email verification
* SQLite database for persistence
* Simple and clean project structure

---

## 🛠 Technologies Used

* Flask
* SQLite
* AWS SES
* HTML (Jinja templates)
* Python Virtual Environment

---

## 📌 Notes

* The `instance/` folder is auto-created when the database initializes.
* Ensure AWS SES is out of sandbox mode to send emails to unverified addresses.

---

## 📄 License

This project is for learning and internal use. Modify as needed.
