# SRM Full Stack Engineering Challenge

Hey! Here is my submission for the Full Stack Challenge. I built this using Node.js & Express for the backend, and standard HTML/CSS/JS for the frontend UI. No massive frameworks, just clean, readable code to get the job done efficiently.

### What's included?
- `backend/server.js`: The Express app containing the API endpoint (`/bfhl`).
- `frontend/index.html`: A simple, responsive frontend to submit test cases and visualize the JSON payload.

### How to Run Locally

**1. Start the API Server**
Open up a terminal and maneuver into the backend folder:
```bash
cd backend
npm install
node server.js
```
*Note: The server defaults to port 3000. It's properly set up with CORS so the frontend can hit it without issues.*

**2. Open the Frontend**
You literally just need to open `frontend/index.html` in your browser. (Double-clicking the file works perfectly).

### Testing the Logic
The frontend's text area is already pre-filled with the exact test cases from the PDF! Just hit **Process Data** and look at the response below it. 

### A quick note on the logic
I used a combination of regular expressions for initial string validation, and a recursive topological-style DFS function to construct the nested JSON trees and calculate edge depths. Duplicates are tracked with Sets, and cycles are aggressively handled so we never hit an infinite loop.

Enjoy! Let me know if you run into any setup snags.