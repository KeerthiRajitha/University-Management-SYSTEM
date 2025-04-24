# University-Management-SYSTEM
# 🎓 College Management System with OTP & Voice Feedback

A command-line Python project to manage colleges, students, and teachers with:
- ✅ OTP-based login via email
- 🔊 Text-to-speech responses for user interaction
## 📁 Project Structure

## 🔧 Features

- 🏫 Add multiple colleges
- 👨‍🎓 Register students (per college)
- 👩‍🏫 Register teachers (per college)
- 📧 OTP-based email login for both roles
- 🗣️ Text-to-speech feedback using `pyttsx3`
---
## ⚙️ Requirements

Install the necessary packages using `pip`:

```bash
pip install pyttsx3
📤 Gmail SMTP Setup (For OTP Emails)
🔐 Enable 2-Step Verification on your Gmail account.

🛠️ Create an App Password from Google Account > Security.

📄 Use this password in the otp_module.py or securely load it from a .env file.

🚀 How to Run
Run the main script:

bash
Copy
Edit
python 1ums.py
📋 Menu Options
text
Copy
Edit
1. Add College
2. Add Student
3. Add Teacher
4. Login as Student (via OTP)
5. Login as Teacher (via OTP)
6. Exit
🛡️ Secure Your Credentials (Recommended)
Avoid hardcoding sensitive information. Use environment variables instead:

1. 📄 Create a .env file:
env
Copy
Edit
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
2. 🧠 Load it in otp_module.py:
python
Copy
Edit
from dotenv import load_dotenv
import os

load_dotenv()

username = os.getenv("EMAIL_USER")
password = os.getenv("EMAIL_PASS")
🗣️ Text-to-Speech
Implemented via pyttsx3:

Provides voice feedback when adding users or logging in

Enhances user interaction in CLI environments
🧠 Notes
Email format is not validated — this can be added for robustness.

Roll numbers and college IDs assume uniqueness — consider enforcing rules or using UUIDs for larger systems.

The project is a starting point for more complex systems like portals or dashboards.
