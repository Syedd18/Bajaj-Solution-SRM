# Bajaj SRM - Full Stack Engineering Challenge

This is my submission for the SRM engineering challenge. I used Node.js with Express for the backend API, and plain HTML, CSS, and JavaScript for the frontend UI.

### Live Demo

- **Frontend URL:** https://bajaj-solution-pi.vercel.app/
- **Backend API:** https://bajaj-solution-api.onrender.com 
*(Note: If you open the backend URL in a browser you will see `Cannot GET /`. This is normal because it only accepts POST requests on the `/bfhl` route.)*

---

### How to run locally

To run the project on your machine:

**1. Start the backend:**
```bash
cd backend
npm install
node server.js
```
*(The server will start on port 3000).*

**2. Open the frontend:**
Open the `frontend/index.html` file in your browser. I added the test cases from the PDF as the default input, so you can click "Process Data" to test it quickly.

---

### How the code works

- **Validation:** The code checks if the input matches the strict `X->Y` format. Invalid strings and duplicate edges are separated into their own lists.
- **Tree Construction & Cycles:** It builds the tree step-by-step using a basic recursive function. It keeps track of visited nodes to find any cycles and prevent infinite loops.
- **Summaries:** It counts the nodes in the longest path to find the tree depth. If two trees have the exact same depth, it compares their root letters alphabetically to break the tie.
