# Campus Event Management System

This is my project submission for the Webknot Campus Drive Assignment.  
The goal of this project is to build a simple **Campus Event Management System** with an **Admin Portal** and a **Student App**.

---

 Project Overview
- **Admin Portal (Web)**: College staff can create and manage events like workshops, fests, hackathons, and seminars.  
- **Student App (Mobile/Web)**: Students can browse upcoming events, register, mark attendance, and submit feedback.  

The project also includes basic reporting features such as event popularity, student participation, and feedback summaries.

---

Tech Stack
- **Frontend**: HTML, CSS, JavaScript (basic UI for now)  
- **Backend**: Node.js / Express (REST APIs)  
- **Database**: SQLite (lightweight, easy to set up)  

---

Features Implemented
1. **Event Management** (Create and List events)  
2. **Student Registration** for events  
3. **Attendance Tracking** (manual check-in)  
4. **Feedback System** (rating 1–5)  
5. **Reports**:
   - Event Popularity Report (by registrations)  
   - Student Participation Report (events attended)  
   - Top 3 Most Active Students (bonus)  

---

 Database Schema
- **Students** (student_id, name, email, college_id)  
- **Events** (event_id, title, type, date, venue, created_by, college_id)  
- **Registrations** (reg_id, student_id, event_id, reg_date)  
- **Attendance** (att_id, student_id, event_id, checkin_time)  
- **Feedback** (feedback_id, student_id, event_id, rating, comments)  

---

API Endpoints
- `POST /events` → Create event  
- `GET /events` → List all events  
- `POST /register` → Register student for event  
- `POST /attendance` → Mark attendance  
- `POST /feedback` → Submit feedback  
- `GET /reports/popularity` → Event Popularity Report  
- `GET /reports/participation` → Student Participation Report  

---

How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   ```
2. Install dependencies:  
   ```bash
   npm install
   ```
3. Run the server:  
   ```bash
   npm start
   ```
4. Access the app at `http://localhost:3000`

---

Assumptions & Limitations
- Students cannot register more than once for the same event.  
- Event IDs are unique only within a college.  
- Attendance must be marked on the event day.  
- Missing feedback does not block reports.  

---

Future Improvements
- Add QR-code based check-in for attendance.  
- Build a proper frontend with React.  
- Add filters in reports (by event type).  

---

## 📸 Demo
👉 Live Project: [My Website](https://lovable.dev/projects/77379c48-16cd-4d9c-bce5-1ce9a83f1220)  
