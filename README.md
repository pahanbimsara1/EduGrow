# 🎓 EduGrow

### Teacher Performance & Development Platform

**EduGrow** is a modern, interactive teacher performance and professional development management platform designed for **Sri Lanka National College**.

It provides a centralized workspace for managing teacher profiles, attendance, professional training, feedback, lesson plans, performance analytics, and recognition.

> **Growing great teachers, together.**

---

## ✨ Overview

EduGrow brings key aspects of teacher performance and professional growth into one dashboard.

The platform supports two main user roles:

* 🛡️ **Administrator**
* 👩‍🏫 **Teacher**

Administrators can monitor faculty-wide performance, while teachers can access their own professional development information, analytics, feedback, attendance, training and lesson plans.

The interface is designed with a clean, responsive dashboard experience and adapts to desktop and mobile screen sizes.

---

## 🚀 Features

### 📊 Dashboard

Provides an overview of teacher performance and development metrics.

Administrators can view:

* Overall faculty performance
* Attendance and punctuality
* Feedback performance
* Professional development progress
* Lesson-plan performance
* Department comparisons
* Performance trends

Teachers receive a personalized dashboard showing their own performance, ranking and development progress.

---

### 👩‍🏫 Teacher Profiles

Manage and explore teacher profiles containing information such as:

* Name
* Subject
* Department
* Qualifications
* Joining date
* Employment type
* Classes taught
* Homeroom
* Mentoring status
* Contact information

Teacher profiles can also be opened in a detailed drawer containing additional performance information.

---

### 🗓️ Attendance Management

EduGrow tracks teacher attendance using statuses such as:

* ✅ Present
* 🟡 Late
* ❌ Absent
* ⚪ Leave

The system calculates:

* Attendance rate
* Punctuality rate
* Attendance score
* Attendance history

Attendance information contributes to the overall performance and recognition system.

---

### 🎓 Training & Certifications

Track professional development activities and certifications.

Training records include:

* Course title
* Training provider
* Category
* Training hours
* Completion status
* Certification information
* Certificate expiry

Example training areas include:

* Differentiated Instruction
* Classroom Assessment
* Digital Tools for Learning
* Inclusive Education
* Advanced Subject Pedagogy
* Data-Driven Instruction
* Mentoring & Coaching
* Child Safeguarding

The platform also monitors professional development hours toward a **40-hour target**.

---

### 💬 360° Feedback

EduGrow supports feedback from multiple sources:

* 👨‍🎓 Students
* 👨‍👩‍👧 Parents
* 👩‍🏫 Peers
* 🛡️ Administrators
* 🙋 Self-evaluation

Feedback includes:

* Rating
* Category
* Comment
* Date
* Feedback source

Feedback contributes to the teacher's overall performance score.

---

### 📐 Lesson Plans

Teachers can create and submit lesson plans for review.

Lesson plans contain:

* Teacher
* Title
* Subject
* Grade
* Date
* Learning objectives
* Review status
* Performance score

Supported statuses include:

* ✅ Approved
* 🔵 Submitted
* 🟡 Needs Revision
* ⚪ Draft

Teachers can submit lesson plans directly for review from the platform.

---

### 📈 Visual Analytics

EduGrow transforms performance data into visual insights.

Analytics include:

* Performance trends
* Attendance analysis
* Punctuality
* Feedback scores
* Training progress
* Lesson-plan quality
* Department comparisons

Department-level comparisons include teacher count, composite performance index, attendance, feedback and professional-development hours.

---

### 🏅 Recognition & Gamification

EduGrow uses a points-based recognition system to encourage continuous professional development.

Teachers can earn points from:

| Category                     | Maximum Points |
| ---------------------------- | -------------: |
| 🗓️ Attendance & Punctuality |            250 |
| 💬 Feedback Ratings          |            300 |
| 🎓 Training & Certification  |            200 |
| 📐 Lesson Plan Quality       |            250 |
| **Total**                    |      **1,000** |

Teachers can also earn achievement badges such as:

* 🏆 Perfect Attendance
* ⏱️ Punctuality Pro
* 📚 Scholar
* 🎖️ Certified Elite
* ⭐ Top Rated
* 📐 Lesson Architect
* 🤝 Mentor
* 🚀 Rising Star

The recognition system includes rankings, growth points and a leaderboard.

---

## 🔐 Authentication

The current project contains a **demo authentication system** with two roles:

### Administrator

```text
Username: admin
Password: admin123
```

### Teacher

```text
Username: teacher
Password: teacher123
```

Teacher login also allows selecting a demo teacher profile.

> ⚠️ **Important:** These credentials are intentionally included in the current demo implementation. This is **not a production-grade authentication system**.

---

## 💾 Data Storage

EduGrow currently operates as a client-side demo application.

### Local Storage

Application data is persisted using browser `localStorage`.

The current storage key is:

```text
edugrow.v3
```

Stored data includes:

* Teachers
* Attendance
* Training records
* Feedback
* Lesson plans

### Session Storage

Login sessions are maintained using:

```text
edugrow.session
```

This means the current version does not require a backend database to run the demo.

---

## 🧠 Performance Scoring

Teacher performance is calculated from four major areas:

```text
Attendance & Punctuality
        ↓
Feedback
        ↓
Training & Certification
        ↓
Lesson Planning
        ↓
Overall Performance Score
```

The current weighting is:

| Area         | Weight |
| ------------ | -----: |
| Attendance   |    25% |
| Feedback     |    30% |
| Training     |    20% |
| Lesson Plans |    25% |

The system also assigns performance grades:

|    Score | Grade |
| -------: | :---: |
|      92+ |   A+  |
|    86–91 |   A   |
|    78–85 |   B   |
|    68–77 |   C   |
| Below 68 |   D   |

---

## 🥇 Teacher Levels

Teachers can progress through four recognition levels:

* 🥉 **Bronze**
* 🥈 **Silver**
* 🥇 **Gold**
* 💎 **Platinum**

Levels are determined by accumulated growth points.

---

## 🎨 Design

EduGrow uses a modern administrative dashboard aesthetic featuring:

* Responsive layout
* Dark navigation sidebar
* Gradient accents
* Card-based UI
* Interactive tables
* Progress bars
* Performance indicators
* Modal dialogs
* Slide-out teacher profiles
* Toast notifications
* Responsive mobile navigation

The interface uses a clean system-font stack and a blue/indigo visual identity.

---

## 📱 Responsive Design

EduGrow is designed to work across:

* 🖥️ Desktop
* 💻 Laptop
* 📱 Mobile
* 📲 Tablet

On smaller screens, the sidebar becomes a collapsible navigation menu and dashboard grids adapt to narrower layouts.

---

## 🛠️ Technology Stack

The current implementation is intentionally lightweight.

### Frontend

* HTML5
* CSS3
* Vanilla JavaScript

### Browser APIs

* `localStorage`
* `sessionStorage`
* DOM APIs

### No Framework Required

The project does **not** currently require:

* React
* Vue
* Angular
* Node.js
* PHP
* Python
* Database server
* Build tools

Everything is contained within the current HTML implementation.

---

## 📂 Project Structure

The current project is implemented as a single HTML file:

```text
EduGrow/
│
└── index.html
```

The file contains:

```text
HTML
├── Login interface
├── Application layout
├── Navigation
├── Dashboard
├── Teacher profiles
├── Attendance
├── Training & certifications
├── Feedback
├── Lesson plans
├── Analytics
├── Recognition
│
├── CSS
│   ├── Layout
│   ├── Components
│   ├── Responsive design
│   └── Animations
│
└── JavaScript
    ├── Application state
    ├── Demo data
    ├── Authentication
    ├── Metrics
    ├── Rendering
    ├── Local storage
    └── User interactions
```

---

## ▶️ Getting Started

### 1. Clone or download the project

Place the project on your computer.

### 2. Open the project

Simply open:

```text
index.html
```

in a modern web browser.

### 3. Sign in

Choose either:

```text
Administrator
```

or

```text
Teacher
```

and use the demo credentials provided above.

No server is required for the current demo.

---

## 🔄 Reset Demo Data

EduGrow includes a **Reset Demo Data** option.

This removes the locally stored application data and restores the generated demo dataset.

This is useful when testing modifications or returning the application to its original demo state.

---

## 🧪 Demo Data

The application generates a deterministic demonstration dataset containing teachers, attendance records, training records, feedback and lesson plans.

The demo environment is intended to demonstrate how EduGrow could work with a larger school dataset without requiring a backend during development.

---

## ⚠️ Current Limitations

This version is a **frontend prototype/demo**, not a production deployment.

Current limitations include:

* Authentication is client-side
* Demo credentials are hard-coded
* Data is stored locally in the browser
* No real database
* No server-side authorization
* No real school information system integration
* No multi-user synchronization
* Demo data is generated locally

Therefore, sensitive or real teacher information should **not** be entered into this version.

---

## 🔮 Future Development

A production version could introduce:

### Backend

* REST API
* Secure authentication
* Role-based authorization
* PostgreSQL / MySQL database
* Server-side validation

### School Integration

* Student information systems
* HR systems
* Attendance hardware
* Existing school databases

### Advanced Analytics

* Predictive performance analysis
* Department-level forecasting
* Professional-development recommendations
* Automated performance reports
* Exportable PDF/Excel reports

### Communication

* Notifications
* Email alerts
* Training reminders
* Certificate-expiry alerts
* Lesson-plan review notifications

### Security

* Password hashing
* Secure sessions
* HTTPS
* Audit logs
* Permission management
* Data encryption

---

## 🎯 Project Vision

EduGrow aims to create a centralized digital environment where teacher performance is not simply measured, but continuously developed.

The platform combines:

**Performance + Professional Development + Feedback + Analytics + Recognition**

into a single school-focused ecosystem.

---

## 🏫 Institution

**Sri Lanka National College** (For Example School)
**Colombo, Sri Lanka**

**Platform:** EduGrow
**Purpose:** Teacher Performance & Professional Development

---

## 📄 License

This project does not currently specify an open-source license.

If you intend to publish the repository publicly, add an appropriate license such as MIT before distributing the project as open source.

---

## 👨‍💻 Development

Built as a modern frontend prototype using pure HTML, CSS and JavaScript.

**EduGrow — Growing great teachers, together.**
