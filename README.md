<p align="center" style="white-space: nowrap; display: inline-block;">
  <img src="https://img.shields.io/badge/Next.js-Frontend-black?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express.js-Backend-grey?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-Database-green?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-Authentication-orange?style=for-the-badge&logo=jsonwebtokens&logoColor=white" />
  <img src="https://img.shields.io/badge/Nodemailer-Email%20Service-blue?style=for-the-badge&logo=gmail&logoColor=white" />
  <img src="https://img.shields.io/badge/Drag%20%26%20Drop-HTML5-red?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge" />
</p>

# Drop2Mail 

**Tagline:** *Drag. Drop. Send.*

Drop2Mail is a productivity tool designed for teachers and administrators.  
It allows you to **drag & drop teachers or groups into a compose zone** and send emails instantly, without the hassle of searching for contacts.

## Features
- Authentication for Admins & Teachers (JWT-based).
- Collections Management: Create, update, and manage groups of students and teachers.
- Students & Teachers: Easily fetch and attach via APIs.
- Drag & Drop to Email: Drop any collection to auto-select recipients.
- Email Sending: Send emails to all students & teachers in a collection.
- Email Logs: Every sent mail is logged with subject, message, and recipients.
- Expandable Recipients View: Dropdown to preview names & emails before sending.


## Tech Stack
🔹 Frontend
- Next.js + TypeScript
- Tailwind CSS (modern responsive UI)
- Drag & Drop API (native HTML5)

🔹 Backend
- Express.js (Node.js framework)
- MongoDB + Mongoose (database & models)
- Nodemailer (email service)
- JWT Authentication

## Folder Structure
```
├── backend
│ ├── config/ # Database connection
│ ├── controllers/ # Route controllers (admin, student, teacher, collection, email)
│ ├── middleware/ # Auth middleware
│ ├── models/ # Mongoose models
│ ├── routes/ # API routes
│ ├── utils/ # Utility functions (sendEmail)
│ ├── server.js # Express app entrypoint
├── frontend
│ ├── src/
│ │ ├── components/ # UI Components (tabs, dashboards)
│ │ ├── pages/ # App Pages (Admin, Teacher)
│ │ ├── assets/ # Static assets
│ │ ├── App.tsx # Main app component
│ │ └── main.tsx # React entrypoint
│ ├── index.html # Vite HTML template
│ └── vite.config.js # Vite config
│
├── README.md # Project documentation
```

## Usage
- Login as Teacher/Admin → Token stored in localStorage.
- View Collections → Fetched via /collection/my.
- Drag & Drop → Drag a collection card into the email drop zone.
- Preview Recipients → Expand dropdown to view all student & teacher emails.
- Send Email → Fill subject & message → Click Send.

## Setup
#### Backend
```
cd backend
npm install
npm run dev
```
#### Frontend
```
cd frontend
npm install
npm run dev
```

## To-Do / Future Enhancements
- [ ] Bulk email scheduling  
- [ ] Attachment support  
- [ ] Rich text editor for email body  


## License
This project is licensed under the MIT License 

