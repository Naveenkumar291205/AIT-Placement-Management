# 🎓 AIT Placement Management System

> A modern student placement management dashboard designed to simplify placement preparation, job applications, recruitment drives, and career tracking.

[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-8-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vite.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Oxlint](https://img.shields.io/badge/Oxlint-Code%20Quality-purple?style=for-the-badge)](https://oxc.rs/docs/guide/usage/linter)

---

## 📌 Overview

**AIT Placement Management System** is a student-focused placement portal created to provide a centralized interface for managing the complete campus placement journey.

The application brings together:

- Student placement dashboard
- Student profile
- Placement applications
- Recruitment drive calendar
- Placement assessments
- Resume building
- Training resources
- Mock interviews
- Certificates
- Leaderboard
- Placement statistics
- Documents
- Notifications
- Placement preparation

The project is designed around a **dashboard-first user experience**, allowing students to access important placement information from a single interface.

---

# 🎯 Objectives

The system aims to improve the campus placement experience by providing students with an organized digital workspace where they can:

```text
Discover Opportunities
        ↓
Review Eligibility
        ↓
Apply for Drives
        ↓
Prepare for Assessments
        ↓
Attend Interviews
        ↓
Track Progress
        ↓
Receive Offers
```

---

# ✨ Features

## 📊 Student Dashboard

The main dashboard provides an overview of the student's placement activity.

### Placement metrics

The dashboard tracks:

- Applied opportunities
- Shortlisted applications
- Upcoming interviews
- Offers received

Example dashboard statistics:

```text
Applied       → 5
Shortlisted   → 2
Interview     → 1
Offers        → 0
```

---

## 🏢 Upcoming Placement Drives

Students can view upcoming recruitment opportunities with information such as:

- Company
- Job role
- CTC
- Drive details
- Application state

The application also provides an **Apply Now** interaction with confirmation through a modal.

---

## 📅 Drive Calendar

A dedicated placement calendar displays recruitment drives and scheduled events.

Example opportunities represented in the application include:

- Zoho Corporation
- Infosys
- TCS
- Accenture
- Cognizant
- Wipro

The calendar interface helps students keep track of recruitment schedules.

---

## 👤 Student Profile

The profile module provides a centralized view of academic and personal information.

Profile information includes:

- Student name
- Degree
- Department
- College
- Batch
- CGPA
- Arrears history
- Email
- Phone
- LinkedIn
- GitHub

---

## 📝 Application Management

The **My Applications** module allows students to monitor their applications.

Application states include:

```text
Apply Now
     ↓
Applied
     ↓
Under Review
```

The interface visually distinguishes applications that have already been submitted.

---

## 🧠 Placement Preparation

A dedicated preparation module is included for placement readiness.

The system provides placement-oriented learning areas such as:

- Aptitude preparation
- Technical preparation
- Interview preparation
- Career training

Preparation modules can be opened through interactive modal windows.

---

## 🔔 Notifications

The application includes a notification system for important placement events.

Example notifications:

```text
Zoho Shortlist Announced
Infosys Drive Registration Closes Soon
Mock Interview Feedback Available
```

Notifications also maintain read/unread state.

---

## 🔍 Search

The dashboard header includes placement-drive search functionality.

Students can search based on:

- Company name
- Job role

Results are dynamically filtered from the drive data.

---

## 🪟 Interactive Modals

The application uses reusable modal-based interactions for:

- Job application confirmation
- Calendar details
- Placement preparation modules
- Additional placement information

This allows users to access details without leaving the dashboard.

---

## 🔔 Toast Notifications

Action feedback is shown using temporary toast messages.

Example:

```text
🎉 Successfully applied for Software Developer!
```

Toast messages automatically disappear after a short period.

---

# 🧭 Navigation Modules

The sidebar currently contains the following placement modules:

| Module | Purpose |
|---|---|
| Dashboard | Placement overview |
| Profile | Student academic and contact information |
| Applications | Track job applications |
| Drive Calendar | Recruitment schedule |
| Assessments | Placement assessment resources |
| Resume Builder | Resume-related functionality |
| Training | Placement training |
| Mock Interview | Interview preparation |
| Certificates | Certification tracking |
| Leaderboard | Performance comparison |
| Placement Stats | Placement analytics |
| Documents | Placement documents |
| Settings | Account preferences |

---

# 🏗️ Application Architecture

The application follows a component-based React architecture.

```text
React Application
│
├── App
│   │
│   ├── Sidebar
│   ├── Header
│   ├── WelcomeBanner
│   ├── StatCards
│   ├── UpcomingDrives
│   ├── PlacementPrep
│   ├── FeatureView
│   │
│   └── Modals
│       ├── ApplyModal
│       ├── CalendarModal
│       └── PrepModal
│
└── Supporting Components
    ├── Icons
    ├── CSS
    └── Assets
```

---

# 📂 Project Structure

```text
AIT-Placement-Management/
│
├── .gitignore
├── .oxlintrc.json
├── README.md
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
│
├── public/
│   ├── favicon.svg
│   └── icons.svg
│
└── src/
    │
    ├── App.jsx
    ├── App.css
    ├── index.css
    ├── main.jsx
    │
    ├── assets/
    │   ├── hero.png
    │   ├── react.svg
    │   └── vite.svg
    │
    └── components/
        ├── FeatureViews.jsx
        ├── Header.jsx
        ├── Icons.jsx
        ├── Modals.jsx
        ├── PlacementPrep.jsx
        ├── Sidebar.jsx
        ├── StatCards.jsx
        ├── UpcomingDrives.jsx
        └── WelcomeBanner.jsx
```

---

# 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| **React 19** | User interface |
| **JavaScript** | Application logic |
| **Vite** | Development and build tooling |
| **CSS3** | Styling and responsive layouts |
| **Oxlint** | JavaScript linting |
| **HTML5** | Application structure |
| **SVG** | Icons and interface assets |

---

# ⚙️ State Management

The current application manages its state with React's built-in `useState` hook.

Important application state includes:

```javascript
activeTab
searchQuery
drives
stats
notifications
selectedDriveToApply
showCalendarModal
selectedPrepModule
toastMessage
```

This provides a lightweight approach suitable for the current frontend implementation.

---

# 🔄 Application Flow

## Dashboard Flow

```text
Student Login / Access
        ↓
Dashboard
        ↓
Placement Statistics
        ↓
Upcoming Drives
        ↓
Apply for Opportunity
        ↓
Application Confirmation
        ↓
Application Status Updated
```

---

## Search Flow

```text
Search Query
     ↓
Company / Role Matching
     ↓
Filtered Drive List
     ↓
Student Reviews Opportunity
```

---

## Application Flow

```text
Upcoming Drive
      ↓
Apply Now
      ↓
Confirmation Modal
      ↓
Confirm Application
      ↓
Application Count Updated
      ↓
Drive Status → Applied & Under Review
```

---

# 🎨 UI / UX Design

The project follows a modern placement-dashboard design with:

- Fixed sidebar navigation
- Dashboard cards
- Status indicators
- Recruitment cards
- Modal-based workflows
- Responsive layouts
- Placement statistics
- Visual notifications
- Consistent iconography
- Card-based information architecture

The design is intended to feel like a **modern student career-management platform** rather than a basic college management page.

---

# 🧩 Reusable Components

The project separates major UI responsibilities into reusable components.

### `Sidebar.jsx`

Responsible for:

- Main navigation
- Active module switching
- Logout interaction

### `Header.jsx`

Responsible for:

- Search
- Notification access
- Header actions

### `StatCards.jsx`

Displays:

- Applications
- Shortlists
- Interviews
- Offers

### `UpcomingDrives.jsx`

Displays:

- Recruitment opportunities
- Company details
- Application actions
- Calendar access

### `PlacementPrep.jsx`

Provides placement preparation modules.

### `FeatureViews.jsx`

Controls module-specific views including:

- Profile
- Applications
- Calendar
- Other placement modules

### `Modals.jsx`

Provides reusable interactive modal components.

---

# 🧪 Development Setup

## 1. Clone the repository

```bash
git clone https://github.com/Naveenkumar291205/AIT-Placement-Management.git
```

## 2. Enter the project

```bash
cd AIT-Placement-Management
```

## 3. Install dependencies

```bash
npm install
```

## 4. Start development server

```bash
npm run dev
```

Vite will display the local development URL in the terminal.

---

# 🏗️ Production Build

Build the application:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

---

# 🧹 Code Quality

The project uses **Oxlint** for linting.

Run:

```bash
npm run lint
```

---

# 📱 Responsive Experience

The interface is designed to support common desktop and smaller-screen layouts.

Responsive considerations include:

- Flexible dashboard grids
- Adaptive navigation
- Responsive cards
- Mobile-friendly spacing
- Scalable typography

---

# 🚀 Deployment

As a Vite React application, the project can be deployed to static frontend hosting platforms such as:

- Vercel
- Netlify
- GitHub Pages
- Cloudflare Pages

---

# 🎓 Target Users

The system is primarily designed for:

- College students
- Placement cells
- Training departments
- Career development teams
- Campus recruitment coordinators

---

# 🏫 Institution Context

The project is designed around a college placement-management use case for:

**Adithya Institute of Technology**

Department-focused placement workflows can be expanded for multiple branches and batches.

---

# 🔮 Future Roadmap

The current repository provides a strong frontend foundation. The next stage can turn it into a complete placement management platform.

### 🤖 AI Features

```text
AI Resume Analyzer
AI Job Recommendation
AI Interview Preparation
AI Skill Gap Analysis
AI Career Assistant
```

### 🏢 Placement Cell Features

```text
Admin Dashboard
Student Management
Company Management
Drive Management
Eligibility Filtering
Recruiter Management
Placement Reports
```

### 📊 Advanced Tracking

```text
Application Timeline
Multi-Round Interview Tracking
Offer Management
Offer Acceptance
Placement Analytics
Department Heatmap
Student Skill Matrix
```

### 📡 Real-Time Features

```text
WebSocket Notifications
Live Drive Updates
Interview Notifications
Placement Announcements
Chat Support
```

### 📄 Document Management

```text
Resume Upload
Offer Letters
Certificates
Placement Documents
Bulk Excel Import / Export
```

---

# 🔐 Recommended Production Improvements

For a production deployment, the current frontend should be extended with:

- Real authentication
- Backend APIs
- Database persistence
- Role-based access control
- Placement-cell admin portal
- Student accounts
- Company accounts
- Secure document storage
- Server-side validation
- Audit logs
- Automated email notifications
- Real-time notifications

---

# 📈 Project Potential

The architecture can evolve from a frontend prototype into a complete **college placement ecosystem**:

```text
                 AIT PLACEMENT PLATFORM
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
     Students          Placement Cell     Companies
        │                 │                 │
        ↓                 ↓                 ↓
    Applications       Drives           Recruitment
    Assessments        Analytics        Candidate Search
    Training           Reports          Feedback
    Interviews         Management       Shortlisting
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ↓
                  Placement Intelligence
```

---

# 👨‍💻 Author

**Naveen Kumar M**

GitHub:  
https://github.com/Naveenkumar291205

---

# ⭐ Project Highlights

- React-based placement dashboard
- Modular component architecture
- Interactive placement applications
- Recruitment drive calendar
- Student placement statistics
- Search and filtering
- Notification system
- Placement preparation modules
- Reusable modal components
- Responsive UI foundation

---

# 📜 License

This project does not currently specify an open-source license.

Add a license such as **MIT** before distributing the project publicly under open-source terms.

---

## 🎯 Vision

> **Make campus placements more organized, transparent, data-driven, and student-friendly.**

**AIT Placement Management System** is designed as a foundation for a smarter digital placement ecosystem where students can manage their entire placement journey from one platform.
