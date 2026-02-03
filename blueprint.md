# Project Blueprint

## Overview

A simple web application with a "Hello, world!" message and a button. This document outlines the plan to add a dark and white mode theme switcher.

## Current State

- `index.html`: Basic HTML structure with a heading and a button.
- `style.css`: Empty.
- `main.js`: Empty.

## Plan for Dark/White Mode

1.  **CSS (`style.css`):**
    -   Define color variables for both light and dark themes using `:root` and `[data-theme='dark']`.
    -   Apply these variables to the `body` and other elements for background and text colors.
    -   Add styles for a theme toggle switch.

2.  **HTML (`index.html`):**
    -   Add a toggle switch element (e.g., a button) to the page to allow users to switch themes.

3.  **JavaScript (`main.js`):**
    -   Implement logic to toggle the `data-theme` attribute on the `<html>` element.
    -   Use `localStorage` to save the user's selected theme and apply it on subsequent visits.

## Partnership Inquiry Form (Formspree)

1.  **Purpose:** To allow users to submit partnership inquiries via a simple contact form, leveraging Formspree for backend processing.

2.  **HTML (`index.html`):**
    -   Added a `<section>` containing a `<form>` element.
    -   The form includes input fields for `name`, `email`, and a `textarea` for `message`.
    -   The form's `action` attribute is set to the provided Formspree endpoint (`https://formspree.io/f/xvzqyzwv`) and `method` to `POST`.

3.  **CSS (`style.css`):**
    -   Added styles for the `.contact-form-section`, `.contact-form`, `.form-group`, `label`, `input`, `textarea`, and `button[type="submit"]` to ensure a clean and responsive appearance, consistent with the existing theme.

## Disqus Comment Section

1.  **Purpose:** To enable a comment section on the page, powered by Disqus, for user engagement.

2.  **HTML (`index.html`):**
    -   Added a `<div id="disqus_thread"></div>` element where the comments will be embedded.
    -   Included the provided Disqus JavaScript snippet, which loads the `embed.js` script from `https://krecipe.disqus.com/embed.js`, responsible for rendering the comment section.
    -   A `<noscript>` fallback message is also included.
    -   **Update:** The Disqus script has been updated to include configuration variables (`this.page.url` and `this.page.identifier`) to improve loading reliability, especially in development environments. The entire integration has also been wrapped in a `<section class="comment-section">` with a `<h2>` for better page structure.

3.  **CSS (`style.css`):**
    -   Added styles for the `.comment-section` to provide appropriate spacing and alignment.
