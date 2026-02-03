CDP CRM Dashboard

A full-stack client dashboard built with Node.js, Express, MongoDB, and Chart.js. This project aggregates client and membership data, demographic analytics, and revenue statistics, then generates an analytic report powered by Gemini AI.

Table of Contents
	•	Features
	•	Project Structure
	•	Deployment
	•	License

Features
	•	Client Statistics:
	•	Total clients
	•	Active memberships
	•	New memberships and clients (October 2024)
	•	Membership vs. non-membership stats and tier breakdown
	•	Demographic Analytics:
	•	National distribution (views by country via a doughnut chart)
	•	Age and gender distribution (displayed as a horizontal bar chart)
	•	Revenue Analytics:
	•	Monthly revenue breakdown for a selected year (split by Membership and General Client)
	•	Summary statistics including total income, average monthly revenue, and average spend rate
	•	Report Generation:
	•	Uses Gemini AI to generate a concise analytic report based on collected metrics

Project Structure

cdp-crm-dashboard/
├── backend/
│   ├── routes/
│   │   ├── clients.js         # Client-related endpoints
│   │   ├── demographic.js     # Demographic endpoints
│   │   ├── generate.js        # Gemini report generation endpoint
│   │   └── promotion.js       # Revenue and promotion endpoints
│   ├── models/
│   │   └── Client.js          # Mongoose model for clients
│   ├── db.js                  # MongoDB connection setup (using environment variables)
│   └── server.js              # Main Express server file
├── frontend/                  # Frontend assets (HTML, CSS, JavaScript)
├── .env                       # Environment variables (MONGODB_URI, GEMINI_API_KEY, API_BASE_URL, PORT)
├── package.json               # Project dependencies and scripts
└── README.md                  # This file

Deployment
	•	Backend: Deploy as a Web Service on Render.
	•	Frontend: Deploy as a Static Site on Render, Netlify, or Vercel.
License

This project is licensed under the MIT License.