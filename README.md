# City General Hospital - Queue Management System

A full-stack implementation of the Hospital Queue Management System using Node.js, Express, MongoDB, and Vanilla HTML/JS.

## 🚀 Key Features

*   **Smart Priority Queue**: Critical patients are automatically prioritized (`C-XXX` tokens vs `S-XXX` tokens).
*   **Real-time Dashboard**: Live updates for Doctors, Admins, and Patients.
*   **Admin Controls**: Reset Queue, View History, Manage Departments.
*   **Wait Time Estimation**: Dynamic calculation based on queue position.
*   **Secure Access**: JWT Authentication for Staff.

## 🛠️ Tech Stack

*   **Backend**: Node.js, Express.js
*   **Database**: MongoDB (In-Memory for Dev, connectable to Atlas)
*   **Frontend**: HTML5, CSS3, Vanilla JS

## 📦 Installation & Setup

1.  **Install Dependencies**
    ```bash
    npm install
    ```

2.  **Start the Server** (Backend)
    ```bash
    # Starts server on port 5000
    node server/server.js
    ```
    *Note: The server uses an In-Memory MongoDB by default. Data is reset on restart.*

3.  **Run the Frontend**
    ```bash
    npm run dev
    ```
    *Opens the application in your browser.*

## 🔑 Default Credentials

| Role | Username | Password |
|---|---|---|
| **Admin** | `adminqueue` | `queue` |
| **Doctor** | `drqueue` | `queue` |

## 🧪 Testing the Flow

1.  **Login as Admin** and hit **Reset Queue** to start fresh.
2.  **Go to Patient Portal (`patient.html`)**:
    *   Register a **Stable** patient (e.g., "John"). Token: `CAR-S-001`.
    *   Register a **Critical** patient (e.g., "Jane"). Token: `CAR-C-001`.
3.  **Check Status**: Jane (Critical) should be **Position 1** and John (Stable) **Position 2**.
4.  **Doctor Portal**: Call Next Patient. It should call **Jane** (Critical) first.

## ⚠️ Admin Reset
Use the red **Reset Queue** button in the Admin Dashboard to wipe all data and reset token counters to 1.
# Hospital Queue Management System

A web-based system designed to manage patient queues efficiently in hospitals. It helps reduce waiting time and improves workflow using separate interfaces for admin and doctors.

## 🔧 Features
- Patient queue management
- Admin dashboard
- Doctor interface
- Simple and user-friendly design

## 💻 Technologies Used
- HTML
- CSS
- JavaScript

## 📁 Project Structure
- index.html – Home page
- login.html – Login page
- admin.html – Admin panel
- doctor.html – Doctor panel

## 🎯 Objective
To improve hospital efficiency by digitizing the patient queue system.

## 👩‍💻 Author
Hima Mariyam
