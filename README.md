📚 Library Management System
A full-stack web application to manage books and members in a library. Built using Flask (Python) for backend and HTML, CSS, JavaScript for frontend, with SQLite for database support and ReportLab for PDF generation.

🛠 Features
📖 Book Management: Add and list available books.

👤 Member Management: Register and list members.

🔁 Borrow/Return System: Borrow books and return them.

💰 Fine Calculation: Calculates overdue fines (₹5/day after 14 days).

📄 PDF Report: Generate borrowing reports per member.

📂 Project Structure
bash
Copy
Edit
├── app.py              # Backend Flask API
├── library.db          # SQLite Database
├── index.html          # Frontend HTML
├── style.css           # Frontend styling
├── script.js           # Frontend JavaScript logic
├── reports/            # Auto-generated PDF reports
└── README.md           # Project documentation
🚀 How to Run
🔧 Prerequisites
Python 3.x

Flask

ReportLab (pip install reportlab)

⚙️ Setup Steps
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/library-management-system.git
cd library-management-system
Install dependencies:

bash
Copy
Edit
pip install flask reportlab
Start the Flask server:

bash
Copy
Edit
python app.py
Open index.html in your browser.

📡 API Endpoints
Method	Endpoint	Description
POST	/api/fine	Calculates fine
GET	/api/report/<member_id>	Generates PDF report for a member
Additional endpoints like /books, /members, /borrow, /return are expected but not yet implemented in app.py as per the JS frontend logic.

✨ To-Do
Add /books, /members, /borrow, /return endpoints in app.py.

Add user authentication (admin/user).

Enhance UI with filters/search.

Deploy to a server (e.g., Heroku or Render).




📄 License
This project is open source and available under the MIT License.
