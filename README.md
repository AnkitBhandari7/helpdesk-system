
# 🎟️ Interactive Help Desk Ticket System

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python)  
![DSA](https://img.shields.io/badge/Data%20Structures-Stack%2C%20Queue%2C%20Heap%2C%20Linked%20List-orange)  
![Status](https://img.shields.io/badge/Status-Active-brightgreen)  
![License](https://img.shields.io/badge/License-MIT-lightgrey)

> 📌 A **Command-Line Help Desk Ticket Management System** built in Python as a **DSA project**.  
> Demonstrates **real-world ticket management** with **Data Structures & Algorithms** such as Stack, Queue, Priority Queue, Linked List, Recursion, and 2D Lists.  

---

## ✨ Features

- 🔑 **Authentication & Roles** → Admin / Staff login via `users.json`  
- 🎟️ **Ticket Management (CRUD)** → Create, View, Process, Undo/Delete  
- 🔄 **Undo Feature (Stack)** → Reopen or delete last ticket action  
- 📊 **Analytics Dashboard (2D List)** → Open vs. Closed, High vs. Normal priority  
- 🔎 **Search & Filter** → By ticket ID, status, or priority  
- 📜 **Ticket History (Linked List)** → Chronological record of all actions  
- 📂 **File Persistence** → Tickets & history saved in `tickets.json`  
- 📑 **Report Generation** → Export tickets & analytics to **Word (.docx)** & **PDF (.pdf)**  

---

## ⚙️ Tech & DSA Concepts
- **Queue (FIFO)** → Normal-priority tickets  
- **Priority Queue (Heap)** → High-priority tickets  
- **Stack** → Undo feature  
- **Linked List** → Ticket history  
- **2D List** → Analytics dashboard  
- **Recursion** → Parent dependency resolution  
- **JSON** → File persistence  

---

## 📂 Project Structure
📦 helpdesk-system
┣ 📜 main.py # Main program file
┣ 📜 tickets.json # Stores tickets + history
┣ 📜 users.json # Stores users & roles
┣ 📜 README.md # Project documentation

## 🚀 Getting Started

### 1️⃣ Clone the Repository

git clone https://github.com/your-username/helpdesk-system.git
cd helpdesk-system

2️⃣ Install Dependencies

pip install python-docx reportlab
3️⃣ Run the Program

python main.py

🔑 Default Users

{
  "admin": {
    "password": "admin123",
    "role": "admin"
  },
  "staff": {
    "password": "staff123",
    "role": "staff"
  }
}
* Admin → Full access
* Staff → Limited access

🧪 Sample Test Cases
Test Case	Input	Expected Output
Create High Priority Ticket	Ticket with priority = High	Added to priority queue
Close Parent Ticket	Close ticket with dependency	Dependent ticket becomes processable
Undo Last Close	Undo command after close	Ticket reverts to open
Filter Open Tickets	Filter by status = open	Shows only open tickets
Search Ticket by ID	Enter Ticket ID = T1	Displays ticket details
📑 Example Report
The system can export Word & PDF reports containing:
* User info (who generated, role, timestamp)
* Tickets list with details
* Analytics Dashboard (stats)
* Ticket history

📌 Future Scope
* 📝 Add user registration via CLI
* 🌐 Integration with MongoDB for multi-user support
* 💻 Web-based frontend (Flask/React)
* 📧 Email notifications for high-priority tickets
* 👨‍💼 Ticket assignment to staff

🏫 Academic Note
This project is part of a Data Structures & Algorithms coursework, focusing on the practical use of:
* Stacks, Queues, Linked Lists, Heaps, Recursion, and File Persistence in Python.

✍️ Author
👨‍💻 Developed by Ankit Bhandari

