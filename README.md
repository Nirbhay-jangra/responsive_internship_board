# Responsive Internship Board — Project Summary

## 1. Project Overview

The Responsive Internship Board is a lightweight, responsive web application developed for the EdVyro Full Stack Development Internship — Task 2.

It helps students discover internship opportunities by browsing listings, searching for relevant roles, and filtering internships by technical domain. The application uses a local JSON dataset and is built entirely with HTML5, CSS3, and Vanilla JavaScript.

## 2. Key Features

- Dynamic internship listings: Displays internship cards generated from JSON data.
- Real-time search: Searches internship titles, domains, locations, work modes, and technical skills.
- Domain filtering: Filters opportunities by Full Stack Development, UI/UX, Data Analytics, and Cyber Security.
- Combined filtering: Applies search and domain filters simultaneously.
- Internship details: Displays role title, domain, work mode, location, number of openings, required skills, and internship reference ID.
- Reset filters: Clears active search terms and selected domain filters.
- Results counter: Shows the number of matching internships.
- Loading state: Displays feedback while internship data is being fetched.
- Empty state: Provides helpful guidance when no internships match the selected filters.
- Error handling: Displays an error message and retry option if the data cannot be loaded.

## 3. Technologies Used

- HTML5: Semantic page structure and accessible form controls.
- CSS3: Responsive layouts, CSS Grid, Flexbox, custom properties, and interactive styling.
- Vanilla JavaScript: Data fetching, filtering, event handling, and dynamic rendering.
- JSON: Stores internship records in a separate local data file.

The project does not require external UI frameworks or JavaScript libraries.

## 4. How It Works

1. The application loads internship records from `internship-records.json`.
2. JavaScript stores the retrieved records in application state.
3. Users search for internships or select a technical domain.
4. The application filters the records based on the selected criteria.
5. Matching internships are displayed as cards.
6. The results counter and active filter indicators update automatically.
7. Loading, empty, and error states provide feedback when necessary.

## 5. Responsive Design

The interface follows a mobile-first approach.

- Mobile (360–480px): Single-column layout with touch-friendly controls.
- Tablet (768–1023px): Two-column card layout and balanced filter controls.
- Desktop (1024px and above): Multi-column internship cards and a wider filter toolbar.

The layout adapts to different screen sizes without requiring a separate mobile application.

## 6. Accessibility Features

- Semantic HTML elements for better structure.
- A skip-navigation link for keyboard users.
- Labels for search and filter controls.
- Visible keyboard focus indicators.
- Screen-reader announcements for result updates.
- Accessible error notifications.
- High-contrast text and controls.
- Keyboard navigation support.

These features help make the application usable for people with different accessibility needs.

## 7. Project Structure

The project contains five main files:

- `index.html` — Page structure and accessibility markup.
- `style.css` — Styling and responsive layouts.
- `script.js` — Data loading, search, filtering, and rendering logic.
- `internship-records.json` — Internship dataset.
- `README.md` — Project documentation and setup instructions.

## 8. How to Run the Project

Because browsers may block JSON fetching from local files, run the project using a local HTTP server.

Recommended method: Open a terminal in the project folder and run:

`python -m http.server 8000`

Then open `http://localhost:8000` in your browser.

Alternatively, use VS Code Live Server or a Node.js local server.

## 9. Testing Checklist

Before submitting the project, verify that:

- Internship records load correctly from the JSON file.
- Search works across all required fields.
- Domain and text filters work together.
- Reset buttons clear the filters.
- Internship cards display all required information.
- Empty and error states work correctly.
- The retry button attempts to reload the data.
- Keyboard navigation and focus indicators work.
- The layout works on mobile, tablet, and desktop.
- No external frameworks or libraries are used.

## 10. Expected Outcome

The final application should provide students with a simple and accessible way to discover relevant internship opportunities. It demonstrates practical skills in responsive web design, DOM manipulation, asynchronous data fetching, search and filtering logic, accessibility, and frontend state management.
