# QuizTech

A Kahoot-inspired interactive quiz platform built for the web. QuizTech lets teachers host live quiz sessions and students join and compete in real time. The project covers a fully designed responsive landing page on the frontend and a Node.js + Socket.io backend for real-time game sessions.

---

## Features

- **Landing page** — responsive hero, "How it works" section, and footer with social links
- **Sign up / Log in** — modal-based authentication forms
- **Create a quiz** — registered users can build quiz games
- **Play a quiz** — join a live session with a PIN (Kahoot-style)
- **Real-time gameplay** — Socket.io syncs questions and answers across all players instantly
- **Responsive navigation** — hamburger menu for mobile, dropdown menus for desktop
- **Contact form** — built-in contact modal

---

## Tech Stack

### Frontend

| Technology | Role |
|---|---|
| HTML5 | Page structure |
| CSS3 / SCSS | Styling and responsive layout |
| Vanilla JavaScript | DOM interactions, modal logic, dropdown menus |
| Font Awesome 4 | Icons |

### Backend

| Technology | Role |
|---|---|
| Node.js | Runtime |
| Express 4 | HTTP server and routing |
| Socket.io 2 | Real-time bidirectional communication |
| MongoDB / Mongoose | Quiz and user data persistence |
| Moment.js | Date/time formatting |

---

## Project Structure

```
QuizTech/
├── index.html          # Main landing page
├── style.css           # Compiled CSS
├── style.scss          # SCSS source
├── package.json        # Node.js dependencies
├── css/
│   └── style.css
└── img/                # Images and assets
    ├── logo.png
    ├── play.png
    ├── share.png
    └── ...
```

---

## How QuizTech Works

```
1. CREATE  — A teacher logs in and creates a quiz (questions + answers)
2. HOST    — Teacher starts a live session; a PIN is generated
3. JOIN    — Students enter the PIN on their device to join
4. PLAY    — Questions appear on the big screen; students answer on their phones
5. RESULTS — Scores are tallied and a leaderboard is displayed in real time
```

---

## Getting Started

### Prerequisites

- Node.js 10+
- MongoDB running locally (or a MongoDB Atlas connection string)

### Install & Run

```bash
# Install dependencies
npm install

# Start the server
npm start
# → Server runs on http://localhost:3000 (or configured port)
```

### Frontend only (no server needed)

Open `index.html` directly in a browser to view the landing page and UI.

---

## Dependencies

| Package | Version | Purpose |
|---|---|---|
| express | ^4.16.3 | Web server |
| socket.io | ^2.1.1 | Real-time events |
| mongoose | ^5.1.5 | MongoDB ODM |
| mongodb | ^3.0.10 | MongoDB driver |
| moment | ^2.22.1 | Date formatting |
