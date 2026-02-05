***Real-time digital clock built with HTML, CSS, and JavaScript demonstrating DOM manipulation, UI updates, and responsive front-end design.

## Colorful Clock — Real-Time Web Application

# Project Overview

This project is a lightweight real-time digital clock built with HTML, CSS, and JavaScript. While simple in concept, it demonstrates core front-end development fundamentals, including DOM manipulation, real-time data rendering, responsive UI design, and animation.

The application dynamically updates the current time every second and visually enhances the display using gradient animations and modern CSS effects.

This project reflects my ability to build interactive, user-facing web applications and translate logic into clean, functional UI behavior.

# Business / Practical Value

Although minimal, this project demonstrates foundational skills used in real-world applications:

 - Real-time UI updates (used in dashboards, monitoring tools, and analytics apps)
 - Dynamic DOM manipulation
 - Clean separation of structure, styling, and logic
 - Front-end responsiveness and visual feedback
 - User interface design using animation and gradients
 - Writing maintainable, readable JavaScript logic

These same concepts scale into production systems such as live dashboards, analytics displays, and web-based tools.

# Technologies Used
 - HTML5 — Application structure
 - CSS3 — Styling, animation, gradients, layout
 - JavaScript — Real-time clock logic and DOM updates

# Features
 - Live digital clock updating every second
 - Automatic 12-hour format conversion (AM/PM)
 - Smooth animated gradient UI
 - Responsive centered layout
 - Lightweight and fast (no libraries required)

# File Structure
 - index.html — Main application structure
 - style.css — Styling, animation, and layout
 - app.js — Clock logic and real-time updates

# How It Works

The application uses JavaScript’s Date() object to retrieve the current system time. A setInterval() function runs every second to:

 - Get the current hours, minutes, and seconds
 - Convert 24-hour time into 12-hour AM/PM format
 - Add leading zeros where needed
 - Update the UI dynamically using DOM manipulation

# Key Logic Example

setInterval(() => {
   const time = document.querySelector(".display #time");
   let date = new Date();

   let hours = date.getHours();
   let minutes = date.getMinutes();
   let seconds = date.getSeconds();
   let day_night = "AM";

   if (hours > 12) {
      day_night = "PM";
      hours = hours - 12;
   }

   hours = hours < 10 ? "0" + hours : hours;
   minutes = minutes < 10 ? "0" + minutes : minutes;
   seconds = seconds < 10 ? "0" + seconds : seconds;

   time.textContent = `${hours}:${minutes}:${seconds} ${day_night}`;
});

# Skills Demonstrated
 - JavaScript logic and real-time execution
 - DOM manipulation
 - Front-end architecture (HTML/CSS/JS separation)
 - UI/UX fundamentals
 - CSS animation and visual styling
 - Writing clean, readable, and maintainable code
