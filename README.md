# React Job Cards UI

A visually focused job listing interface built with **React.js and Vite**, featuring reusable job cards, a looping video background, glassmorphism styling, and interactive visual states.

## Overview

This project is a frontend UI implementation for displaying job opportunities in a card-based layout.

Each job card presents information such as the company, job role, posting date, employment type, experience level, hourly rate, and location.

The interface combines reusable React components with a video background and translucent glass-style cards to create an immersive job listing experience.

---

## Features

* 💼 Job listing card interface
* 🔄 Reusable React card component
* 🏢 Company logos and job information
* 📅 Job posting dates
* 🏷️ Employment type and experience-level tags
* 💰 Hourly compensation display
* 📍 Job location display
* 🎥 Full-screen looping video background
* ✨ Glassmorphism-inspired card styling
* 🖱️ Hover animations and visual effects
* 🔖 Save button interface
* 🎯 Apply Now button interface
* ⚡ Vite-powered development environment

> **Note:** The Save and Apply Now buttons are currently UI elements and do not perform data saving or application actions.

---

## Tech Stack

| Technology   | Purpose                                         |
| ------------ | ----------------------------------------------- |
| React.js     | Building the user interface                     |
| Vite         | Development server and build tooling            |
| JavaScript   | Application logic and data handling             |
| CSS          | Layout, styling, animations, and visual effects |
| Lucide React | Bookmark icon used in the card interface        |

---

## Project Structure

```text
react-job-cards-ui/
│
├── public/
│   └── background.webm
│
├── src/
│   ├── components/
│   │   └── Cards.jsx
│   │
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

---

## How It Works

The project stores the job listing data in `App.jsx`.

Each job entry contains information including:

```text
Company
Company Logo
Date Posted
Job Title
Employment Type
Experience Level
Hourly Pay
Location
```

The data is mapped into reusable `Cards` components.

The `Cards` component receives the job information through React props and renders the corresponding job card.

### Component Flow

```text
App.jsx
   │
   ├── Job Data
   │
   └── Maps Job Data
          │
          ▼
      Cards.jsx
          │
          ▼
      Job Card UI
```

---

## Installation

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project

```bash
cd react-job-cards-ui
```

### 3. Install dependencies

```bash
npm install
```

---

## Run Locally

Start the Vite development server:

```bash
npm run dev
```

Vite will provide a local development URL in the terminal.

Open that URL in your browser to view the project.

---

## UI Highlights

### Reusable Job Cards

The job listing interface uses a dedicated `Cards` component that receives job information through props.

This keeps the card markup reusable instead of duplicating the same HTML structure for every job.

### Video Background

The interface uses a fixed looping video background:

```text
/public/background.webm
```

The video is muted, automatically played, and positioned behind the main card layout.

### Glassmorphism Styling

The cards use translucent backgrounds, backdrop blur, rounded borders, and shadows to create a glass-style visual appearance.

### Hover Effects

Cards have a hover interaction that changes their position, border appearance, and glow effects.

---

## Responsive Behavior

The layout uses a flexible wrapping container so cards can move onto additional rows as the available screen width decreases.

The project is primarily designed around the desktop layout. Small-screen responsiveness may require additional CSS adjustments for narrower mobile viewports.

---

## Data

The displayed job listings are static data defined directly inside `App.jsx`.

This project does not currently use:

* A backend
* A database
* An external job listings API
* User authentication
* Persistent saved jobs
* Functional job application processing

---

## Current Limitations

The current version focuses on the visual frontend implementation.

The following functionality is not implemented:

* Persistent Save functionality
* Job application processing
* Backend integration
* Database storage
* Authentication
* External job API integration

---

## Development

To run the project locally during development:

```bash
npm run dev
```

The application uses Vite for the local development environment.

---

## License

This project is intended as a frontend development project and learning implementation.

---

## Author

**Rafay Amir**

Built with React.js, Vite, JavaScript, and CSS.
