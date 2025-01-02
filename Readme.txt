Calendar Tracking Application
Overview
This is a React-based application that provides calendar tracking functionality with interactive features, leveraging FullCalendar and various modern web development tools.

Setup Instructions
Prerequisites
Ensure the following tools are installed on your system:

Node.js (>= 16.x)
npm (>= 8.x)
A modern browser (Chrome, Firefox, Edge, etc.)
Installation
Clone the repository: bash git clone cd
Install dependencies: bash npm install
Running the Application
Start the development server: bash npm run dev
Open the application in your browser at http://localhost:5173 (default port for Vite).
Building for Production
Generate the production build: bash npm run build
Serve the production build locally: bash npm run preview
Deploy the contents of the dist/ folder to your preferred hosting provider.
Testing
Run linter and tests: bash npm run lint

Deployment
This application is optimized for deployment on static hosting platforms such as:

Netlify
Vercel
GitHub Pages
Steps:
Build the production version: bash npm run build

Deploy the dist/ folder to the hosting platform.

Application Functionality
Features
Interactive Calendar:

Display events using FullCalendar.
Supports drag-and-drop and event resizing (via @fullcalendar/interaction).
Event Management:

Add, edit, and delete events.
Responsive UI with Tailwind CSS.
State Management:

Utilizes Zustand for efficient state management.
Data Handling:

Caches server-state using React Query.
Uses date-fns for flexible date manipulation.
Known Limitations
Timezone Sensitivity: Event times may behave unpredictably across different timezones.
Limited Browser Compatibility: Optimized for modern browsers; older versions may not work fully.
Folder Structure
├── public/
├── src/ │ ├── components/
│ ├── pages/
│ ├── store/
│ ├── types/
│ └── main.tsx
└── package.json

Contributing
Fork the repository.
Create a feature branch: git checkout -b feature-name
Commit changes: git commit -m 'Add feature-name'
Push to the branch: git push origin feature-name
Submit a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for details.
