# The Word Within (TWI) - Bible API Project

## Overview

The **The Word Within (TWI)** project is a web-based application that allows users to explore the Bible interactively. It provides features such as selecting Bible versions, navigating books, chapters, and verses, searching for specific passages, and viewing detailed content. The application integrates with the [Scripture API](https://scripture.api.bible/) to fetch Bible data dynamically.

## Features

1. **Bible Version Selection**: Users can select from a list of Bible versions available in English.
2. **Book Navigation**: Users can browse books of the Bible for the selected version.
3. **Chapter and Verse Navigation**: Users can view chapters and verses within a book.
4. **Search Functionality**: Users can search for specific verses or keywords across the Bible.
5. **Dynamic Content Rendering**: The application dynamically fetches and displays Bible content using the Scripture API.

## Project Structure
root/ 
├── app.js 
├── public/ │ 
    ├── HTML files (e.g., index.html, verse.html) │ 
    ├── css/ │ │ 
        ├── main.css │ │ └── scripture.css │ 
    └── js/ │ 
        └── my_key.js 
├── .env.development 
├── package.json 
└── readme.md


### Key Files

- **`app.js`**: The main server file that serves static files from the `public` directory using Express.js.
- **`public/`**: Contains the HTML, CSS, and JavaScript files for the client-side application.
  - **HTML Files**: Each file corresponds to a specific page in the application (e.g., `index.html` for the homepage, `verse.html` for viewing verses).
  - **CSS Files**: Stylesheets for the application (`main.css` for general styles, `scripture.css` for Bible content formatting).
  - **JavaScript Files**: Contains the API key (`my_key.js`) and client-side logic embedded in the HTML files.
- **`.env.development`**: Stores environment variables (e.g., API keys) for local development.
- **`package.json`**: Defines the project dependencies and scripts.

## How It Works

1. **Server Setup**: The server is built using Express.js and serves static files from the `public` directory.
2. **API Integration**: The application uses the Scripture API to fetch Bible data. The API key is stored in `my_key.js`.
3. **Dynamic Navigation**:
   - Users can navigate through Bible versions, books, chapters, and verses.
   - Breadcrumbs are dynamically generated to show the user's navigation path.
4. **Search Functionality**: Users can search for specific verses or keywords. Results are displayed with links to view the full chapter or passage.
5. **Responsive Design**: The application is styled to be responsive and user-friendly across devices.

## Getting Started

### Prerequisites

- Node.js and npm installed on your system.

### Install Dependencies
```
npm install
```

### Start the server
```
npm start
nodemon app.js
```
### Open browser to:
```
http://localhost:8000
```

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd bible-api




