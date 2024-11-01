# Sports News Website

## Overview
This project is a comprehensive, interactive sports news website designed to keep users up-to-date with the latest developments in various sports. The site includes individual pages for different sports categories: the main homepage, football news, contact page, and a detailed page for a recent CSKA victory. Each page is styled consistently and incorporates interactive features to enhance user experience, such as theme switching, real-time date and time display, and a rating system.

## Project Structure

### Pages
1. **index.html** - The homepage showcasing the latest sports news.
2. **football.html**(basketball,tennis) - Dedicated page for football news with filtering options.
3. **contacts.html** - Contact page providing users with ways to connect with the editorial team.
4. **details.html** - A detailed page on CSKA’s victory, with a built-in rating system for users to score the video.

### Directory Structure
The following is an ideal structure to organize the files:

Organizing files in this structure will help maintain a clean and scalable project as the application expands.

## Features and Functionality

### Homepage (`index.html`)
- **Navigation Bar**: Links to each main section (Homepage, Football, Basketball, Tennis, Contacts).
- **Theme Toggle**: A button to switch between light and dark themes, with the choice saved in `localStorage` so it persists across sessions.
- **Real-time Date & Time Display**: Current date and time displayed and updated every second.
- **Interactive News Cards**: Cards for each news category that enlarge and add a shadow effect on hover for better visual appeal.
- **Background Music**: Play and pause button for background music that can be toggled by users.
- **Accordion FAQ Section**: Frequently Asked Questions (FAQ) section where each question expands to show an answer, navigable with "Next" and "Back" buttons.

### Football(basketball,tennis) News Page (`football.html`)
- **News Filtering**: Users can filter football news based on categories such as “RPL,” “World Cup,” and “Euroleague.” Each filter displays relevant articles only.
- **Persisting Filter Selection**: The last selected filter is saved in `localStorage` to restore the choice when the user revisits the page.
- **Theme Toggle**: Similar theme toggle functionality as on the homepage.

### Contact Page (`contacts.html`)
- **Contact Form with Validation**: Allows users to submit their name, email, and message. Each field is validated, and error messages display if any data is missing or invalid.
- **Popup Modal**: The contact form appears as a popup window with a dimmed background overlay for focus. The popup can be opened and closed by buttons.
- **Language Selector**: Users can choose their preferred language (Russian, English, or Kazakh) for the contact form.
- **Form Reset**: A "Clear" button is provided to reset all input fields in the contact form.
- **Client-Side Form Validation**: JavaScript is used to validate the form fields before submission to ensure correct data entry.

### Details Pages (`details.html`)
- **Video Embedding**: A video player embedded on the page, with autoplay and interaction controls.
- **Rating System**: A star-based rating system where users can rate the video from 1 to 5 stars. The selected rating updates the text below to reflect the user’s score (e.g., "1 star - Very Poor").
- **Navigation Menu**: A consistent navigation menu allows users to move to other sections of the website easily.

## Technologies Used
- **HTML5**: For the structure and layout of the web pages.
- **CSS3**: For styling the pages, including light and dark themes, hover effects, responsive design, and more.
- **JavaScript**: Enables interactive features, including the theme toggle, date and time update, FAQ accordion, filtering, form validation, and star rating.
- **Bootstrap 4.5.2**: Used for styling elements, layout responsiveness, and built-in components like buttons and grids.

## JavaScript Functionalities
Each page contains JavaScript that enhances interactivity:

1. **Theme Toggle (all pages)**: 
   - Toggles between light and dark themes.
   - Saves the user’s choice in `localStorage` to persist the selected theme across sessions.

2. **Date & Time Display (all pages)**: 
   - Updates every second using `setInterval` to keep the date and time accurate.

3. **Accordion Navigation (index.html)**:
   - Implements a multi-step FAQ accordion that displays answers to common questions one at a time.

4. **News Filtering (football.html)**:
   - Displays only relevant news based on user-selected filters.
   - Saves filter selection to `localStorage` to load the same filter on return visits.

5. **Popup Form & Validation (contacts.html)**:
   - Opens a form in a popup modal for users to submit messages.
   - Validates fields, ensuring correct data is provided before submission.

6. **Star Rating System (details.html)**:
   - Users can rate the video using a 1-5 star system.
   - Changes star colors to gold when selected and displays a relevant message based on the rating.

## Instructions for Running the Project
1. Clone or download the project repository.
2. Ensure all HTML files (`index.html`, `football.html`, `contacts.html`, `details.html`) and CSS/JS files are located in the correct directory structure as shown above.
3. Open `index.html` in a browser to start exploring the website.
4. Navigate through the various sections using the links in the navigation bar.
5. Keyboard Events: The script listens for keydown events specifically for the ArrowRight and ArrowLeft keys.
Focus Movement:
Right Arrow: Moves focus to the next menu item.
Left Arrow: Moves focus to the previous menu item.
Wrapping: If the focus reaches the last menu item and the user presses ArrowRight, focus wraps around to the first item. Similarly, pressing ArrowLeft on the first item moves focus to the last item.
Initial Focus on Page Load: The script automatically sets the focus to the first menu item when the page loads, improving user navigation and accessibility from the start.

## Suggested Improvements and Future Enhancements
- **Dynamic Content from an API**: Integrate with a sports news API to fetch live sports updates and results.
- **Database Integration**: Add a backend to store user messages from the contact form and save ratings for each video.
- **User Authentication**: Add login functionality so users can have personalized settings saved (like theme choice and favorite categories).
- **Advanced Filtering and Search**: Implement advanced filtering options and a search bar for users to find specific articles or content more easily.
- **Comments Section**: Allow users to leave comments on each news article, providing a community feel.

## Folder Organization
To ensure clean code and scalability, a sample directory structure is recommended as follows:

## License
All rights reserved. © 2024 Sports News. Redistribution or use of this project without explicit permission is prohibited.


