📌 IntelliSQL – Text to SQL using Gemini LLM

IntelliSQL is an AI-powered web application that converts natural language questions into SQL queries and executes them on a MySQL database. It helps users interact with databases without writing SQL manually by using Google Gemini Large Language Model.

 **Features**

* Converts English questions into SQL queries automatically

* Executes generated SQL queries on a MySQL database

* Displays results in a user-friendly web interface

* Built using Python, Streamlit, and Gemini LLM

 **Technologies Used**
* Python

* Streamlit

* Google Gemini LLM

* MySQL

* dotenv (for environment variables)

📂 Project Structure

intellisql/

 |

├── app.py

├── db.py

├── requirements.txt

└── .env

**Installation & Setup**

 **1: Clone the Repository**

* git clone https://github.com/lakshmiaravind1234/intellisql.git

* cd intellisql

 **2: Install Dependencies**
 
 * pip install -r requirements.txt

**3: Configure Environment Variables**

  * **Create a .env file and add:**

  * GEMINI_API_KEY=

  * DB_HOST=localhost

  * DB_USER=root

  * DB_PASSWORD=your_mysql_password

  * DB_NAME=intellisql

**4: Database Setup (MySQL)**

CREATE DATABASE intellisql;

USE intellisql;

CREATE TABLE students (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(50),
  branch VARCHAR(50),
  marks INT
);

INSERT INTO students (name, branch, marks) VALUES

('Arjun', 'CSE', 85),

('Priya', 'ECE', 90),

('Ravi', 'MECH', 75);

**5: Run the Application**

streamlit run app.py


**6: Open in browser:**

http://localhost:8501


🧪 Example Query

Show all students who scored more than 80

📌 Use Cases

* Helps non-technical users query databases

* Reduces manual SQL writing

* Useful for data analysis and educational purposes

📜 License

* This project is created for educational and learning purposes.

👤 Author

Lakshmi Aravind Reddy Ummadi
