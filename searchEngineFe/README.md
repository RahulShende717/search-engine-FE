# Frontend: Parquet Search Engine UI

This is the frontend part of the full-stack Parquet Search Engine project.  
Built using **ReactJS** and **Vite**, it provides a simple user interface to:

- Upload `.parquet` files to the backend server
- Search records dynamically with a debounce mechanism
- Display matching results cleanly





# Features

1.  Upload Parquet File
  Upload a `.parquet` file from your local machine to the backend using a form.

2. Debounced Search 
  Search input field with **0.5-second debounce** to avoid overloading the backend while typing.

3. Display Search Results
  Cleanly shows matched records (e.g., Message, Tag, Sender) dynamically as the user searches.

4. Error Handling 
  Alerts for missing file uploads, server errors, and search issues.




# Architecture Overview

1. Frontend Framework: [ReactJS]
2. HTTP Client: [Axios]
3. UI Strategy: Simple and responsive HTML/CSS without heavy styling frameworks.




# How to Build and Run the Application

1. Prerequisites -- [Node.js]
2. Backend server running at 4000




# Install Dependencies

1. npm install
2. npm run dev
3. http://localhost:5173




# API Integration

1. post - 	/upload                      -  Uploads a .parquet file to backend
2. get - 	/search?query=your_keyword   -  Searches records matching the query



# Design Choices

1. ReactJS with Functional Components: Modern approach with hooks for state management.
2. Axios for API Calls: Simplified HTTP communication with backend.
3. Debounced Search Logic: Implemented using useEffect and setTimeout to delay API requests after typing.
4. Minimalist UI: Simple HTML/CSS with easy extensibility for future frameworks like Material-UI.


# Performance Optimizations

1. Debouncing: Waits for 2 seconds of inactivity before firing search API requests.
2. Error Boundaries: Catches and displays alert messages for any upload or search errors.
3. Optimized Render: Minimal re-renders when typing or uploading.



