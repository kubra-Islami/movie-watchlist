# 🎬 Movie Watchlist Manager (React)

A scalable and user-friendly **React application** for managing a personal movie watchlist.  
This project focuses on **state-driven UI**, **user interaction**, and **derived data**, while being designed to grow into a more advanced application over time.

---

## ✨ Overview

Movie Watchlist Manager helps users organize movies they want to watch, track viewing progress, and filter content dynamically.

The application is intentionally built with a **clean architecture** and **clear state flow**, making it easy to extend with new features such as persistence, APIs, or animations.

---

## 🎯 Project Goals

- Demonstrate strong React fundamentals
- Build a UI driven entirely by state
- Use derived state instead of redundant stored values
- Keep components reusable and maintainable
- Provide a solid foundation for future expansion

---

## 🧩 Features

### Movie Management
- Add movies with a title and genre
- Mark movies as watched or unwatched
- Remove movies from the list

### Filtering
- Filter movies by status:
  - All
  - Watched
  - Unwatched
- Instant UI updates based on the selected filter

### Live Statistics (Derived State)
- Total movies
- Watched movies count
- Unwatched movies count

All statistics are computed dynamically from the current movie list.

### Smart UI Feedback
- Displays a message when no movies match the selected filter
- Shows a completion message when all movies are watched

---

## 🏗️ Architecture & Concepts

This project follows modern React best practices:

### State Management
`useState` is used for:
- Movies list
- Form inputs
- Active filter

Derived values are **not stored in state**.

### Derived State
Computed during render using:
- `.filter()`
- `.length()`

Examples include:
- Filtered movie list
- Watched and unwatched counts
- Total movie count

### Rendering Lists
- Movies are rendered using `.map()`
- Each movie has a stable and unique ID
- Proper `key` usage (no array index)

### Event Handling
- `onChange` for inputs and selects
- `onClick` handlers for:
  - Adding movies
  - Toggling watched status
  - Deleting movies
  - Switching filters

---

## 📁 Project Structure

```txt
src/
│── components/
│   ├── MovieForm.jsx
│   ├── MovieList.jsx
│   ├── MovieItem.jsx
│   ├── FilterControls.jsx
│   └── Summary.jsx
│
│── App.jsx
│── main.jsx
│── styles.css
```

## 🚀 Getting Started
### Clone the repository:
`git clone <repository-url>
`
### Install dependencies:
`npm install
`

### Run the project:
`npm run dev
`

## 🛠️ Tech Stack
- React
- JavaScript (ES6+)
- JSX
- CSS
- Vite

## 🤝 Contributions

Suggestions, improvements, and feature ideas are welcome.
This project is designed to evolve over time.
