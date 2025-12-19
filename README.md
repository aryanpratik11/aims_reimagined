# AIMS Reimagined 🎓

**AIMS Reimagined** is a high-performance, mobile-first Academic Information Management System. It modernizes the student experience by providing a clean, intuitive interface for managing academic records, course registration, and placement opportunities.

Built as a **Progressive Web App (PWA)**, it offers a native-app feel on both desktop and mobile, ensuring students can access their data anytime, even with limited connectivity.

---

## 🚀 Core Features

* **Smart Dashboard:** At-a-glance view of GPA, attendance, pending fees, and upcoming events.
* **Intelligent Course Registration:** Real-time credit validation, seat availability tracking, and "Add/Drop" functionality with automated deadline logic.
* **Career & Placements:** Integrated portal for job applications, resume management, and CGPA-based eligibility filtering.
* **Account Management:** Self-service profile with document uploads (Aadhaar, Marksheets) and admin-locked official fields.
* **Performance Tracking:** Detailed semester-wise grade breakdowns and cumulative GPA calculations.
* **PWA Integration:** Fully installable with offline caching via Service Workers.

---

## 🛠️ Tech Stack

* **Library:** React 19 (Latest)
* **Styling:** Tailwind CSS (Utility-first CSS)
* **Routing:** React Router 7
* **Icons:** Lucide React & Heroicons
* **State:** LocalStorage-based persistence (Mock Backend)
* **PWA:** Service Workers, Manifest API

---

## 🎨 UI/UX Design: Nielsen’s 10 Usability Heuristics

This project was developed with a strict focus on **Jakob Nielsen’s 10 Usability Heuristics** to ensure a friction-less user experience.

| Heuristic | Implementation in AIMS Reimagined |
| --- | --- |
| **#1: Visibility of system status** | Progress bars in Course Registration show live credit limits; status badges (Applied, Pending, Resolved) update instantly. |
| **#2: Match between system and real world** | Uses standard academic terminology (Credits, CGPA, Backlog, Semester) and logical iconography (briefcase for jobs, heart for favorites). |
| **#3: User control and freedom** | Students can "Drop" courses before submission and use the "Cancel" button in Account settings to undo changes without saving. |
| **#4: Consistency and standards** | Standardized layout components (Sidebar/Navbar) and button styles ensure a predictable interface across all 10+ pages. |
| **#5: Error prevention** | Logic prevents adding courses if credits exceed the limit or seats are full. Login requires a math-based captcha to prevent bot errors. |
| **#6: Recognition rather than recall** | Tooltips (ⓘ) on course tiles show full details on hover, so users don't have to memorize prerequisites or faculty names. |
| **#7: Flexibility and efficiency of use** | Search bars and multi-filters (Category/Semester) allow students to find specific courses or companies in seconds. |
| **#8: Aesthetic and minimalist design** | A card-based UI removes clutter. Secondary information is hidden in modals (e.g., Company details) to maintain focus. |
| **#9: Help users recognize/recover from errors** | Visual feedback for failed logins and clear red text indicators for "Limit Exceeded" or "Incorrect Captcha." |
| **#10: Help and documentation** | Important dates are highlighted in the Registration and Inbox pages, acting as a guide for time-sensitive tasks. |

---

## 📦 Getting Started

### Prerequisites

* Node.js (v18 or higher)
* npm or yarn

### Installation

1. **Clone the repo:**
```bash
git clone https://github.com/your-username/aims-reimagined.git
cd aims-reimagined

```


2. **Install dependencies:**
```bash
npm install

```


3. **Run the App:**
```bash
npm start

```


Open [http://localhost:3000](https://www.google.com/search?q=http://localhost:3000) to view it in the browser.

---

## 📁 Project Structure

```text
src/
├── components/     # Atomic UI components (Buttons, Inputs, Modals)
├── data/           # Mock databases (Users, Courses, Placements)
├── layouts/        # Shared page structures (Sidebar/Navbar wrappers)
├── pages/          # Individual route views (Dashboard, Account, etc.)
├── utils/          # Auth logic, Mock API wrappers, and helpers
└── App.js          # Main router and Protected Route configuration

```

---

## 📱 PWA Features

* **Installable:** Prompts users to "Install App" for a standalone experience.
* **Service Worker:** Caches essential assets (icons, manifest, index.html) for faster load times.
* **Responsive:** Fully optimized for mobile, tablet, and desktop viewports.

