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
