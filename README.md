# Blockchain-based-System-monitoring-State-government-Schemes
A Django-based DApp integrating Web3.py and Ganache to monitor and manage state government welfare fund schemes. Ensures transparent fund allocation, secure blockchain-backed transactions, and role-based access for governments and organizations.
# Blockchain-Based System Monitoring State Government Schemes

A decentralized web application built using Django, Web3.py, and Ethereum (Ganache) to ensure transparent and secure fund allocation for state government welfare schemes.

## 🚀 Features

- Role-based login for:
  - State Government (add/allocate funds)
  - Organizations (request/view funds)
  - Users (sign-up and dashboard)
- Ethereum smart contracts for secure, tamper-proof transactions
- Web3.py integration to connect Python backend with blockchain
- MySQL for storing user and transaction data
- Django templates with responsive design

## 🔧 Tech Stack

- **Frontend**: HTML, CSS, Bootstrap
- **Backend**: Python (Django)
- **Blockchain**: Ethereum, Ganache, Solidity, Web3.py
- **Database**: MySQL

## 🎯 Objectives

- Increase transparency in welfare fund distribution
- Prevent fund misallocation
- Enable real-time monitoring using blockchain technology

## 🛠️ Setup Instructions

1. Clone the repository
2. Set up and run Ganache
3. Compile and deploy smart contracts
4. Configure Django `settings.py` and MySQL database
5. Run Django server:  



Steps to run this project

## ▶️ How to Run the Project

Follow these steps to set up and run the project locally:

1. **Clone the Repository**
   ```bash
   git clone <your-repo-url>
   cd <project-folder>
2. Set Up a Virtual Environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4.Start Ganache
Open Ganache and start a new workspace.
Note the RPC server URL (usually http://127.0.0.1:7545) and contract addresses.
5.Compile & Deploy Smart Contracts
If using solcx, write a deployment script using Web3.py
Update contract ABI and address in your Django app
6.Configure MySQL Database
Create a MySQL database (e.g., gov_schemes_db)
Update settings.py:
python
Copy
Edit
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'gov_schemes_db',
        'USER': 'your_mysql_user',
        'PASSWORD': 'your_mysql_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
7.Run Migrations
bash
Copy
Edit
python manage.py makemigrations
python manage.py migrate
8.Create Superuser (Optional)
bash
Copy
Edit
python manage.py createsuperuser
9.Start the Django Server
bash
Copy
Edit
python manage.py runserver
10.Access the App
Visit http://127.0.0.1:8000/ in your browser.
