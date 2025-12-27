🎂 Automated Birthday Wisher (Python)
This project automatically sends Happy Birthday emails to people whose birthday matches the current date.
It uses Python, Pandas, SMTP, and randomized email templates.

🚀 Features


Reads birthday data from a CSV file


Checks if today matches any birthday


Sends an automated birthday email


Uses random letter templates


Fully automatic (can be scheduled daily)



🛠️ Technologies Used


Python 3


Pandas


smtplib


datetime


random



📁 Project Structure
birthday-wisher/
│
├── main.py
├── birthdays.csv
├── letter_templates/
│   ├── letter_1.txt
│   ├── letter_2.txt
│   └── letter_3.txt
└── README.md


📄 birthdays.csv Format
name,email,year,month,day
Mohit,mohit@gmail.com,1999,12,27
Rahul,rahul@gmail.com,2000,5,10


✉️ Letter Template Format
Each letter file must contain:
Dear [NAME],

Happy Birthday! 🎉
Have a great year ahead.

Regards,
Your Friend

[NAME] will be replaced automatically.

⚙️ Setup Instructions
1️⃣ Install Required Library
pip install pandas


2️⃣ Update Email Credentials
In main.py, replace:
MY_EMAIL = "your_email@gmail.com"
MY_PASSWORD = "your_app_password"

⚠️ Important:
For Gmail, you must use App Password, not your normal password.

3️⃣ Update SMTP Server
For Gmail:
smtplib.SMTP("smtp.gmail.com", 587)

For others:


Outlook: smtp.office365.com


Yahoo: smtp.mail.yahoo.com



4️⃣ Allow Email Access


Enable App Passwords in Gmail


OR allow less secure apps (not recommended)



5️⃣ Run the Program
python main.py


🔄 How It Works


Gets today’s date


Reads birthday data from CSV


Matches today’s month & day


Selects a random birthday letter


Sends an email automatically 🎉



⏰ Automation (Optional)
You can schedule this script:


Windows: Task Scheduler


Linux/Mac: Cron Job


Run it once daily.

📌 Note


Internet connection required


Email credentials must be correct


CSV date must match today's date to send mail



⭐ Future Improvements


WhatsApp/SMS integration


GUI version


Multiple birthdays per day


Email attachments


👨‍💻 Author
Mohit Gupta
Learning Python | Automation | Projects
