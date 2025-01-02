# Calendar Tracking Application

## Overview
This is a React-based application that provides calendar tracking functionality with interactive features, leveraging FullCalendar and various modern web development tools.

## Setup Instructions

### Prerequisites
Ensure the following tools are installed on your system:
- Node.js (>= 16.x)
- npm (>= 8.x)
- A modern browser (Chrome, Firefox, Edge, etc.)

### Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Running the Application
1. Start the development server:
   ```bash
   npm run dev
   ```
2. Open the application in your browser at `http://localhost:5173` (default port for Vite).

### Building for Production
1. Generate the production build:
   ```bash
   npm run build
   ```
2. Serve the production build locally:
   ```bash
   npm run preview
   ```
3. Deploy the contents of the `dist/` folder to your preferred hosting provider.

### Testing
Run linter and tests:
```bash
npm run lint
```

## Deployment
This application is optimized for deployment on static hosting platforms such as:
- Netlify
- Vercel
- GitHub Pages

### Steps:
1. Build the production version:
   ```bash
   npm run build
   ```
2. Deploy the `dist/` folder to the hosting platform.

## Application Functionality

### Features
- **Interactive Calendar:** 
  - Display events using FullCalendar.
  - Supports drag-and-drop and event resizing (via `@fullcalendar/interaction`).

- **Event Management:**
  - Add, edit, and delete events.
  - Responsive UI with Tailwind CSS.

- **State Management:**
  - Utilizes Zustand for efficient state management.

- **Data Handling:**
  - Caches server-state using React Query.
  - Uses `date-fns` for flexible date manipulation.

### Known Limitations
- **Timezone Sensitivity:** Event times may behave unpredictably across different timezones.
- **Limited Browser Compatibility:** Optimized for modern browsers; older versions may not work fully.

## Folder Structure
```
├── public/           # Static assets
├── src/
│   ├── components/   # Reusable React components
│   ├── pages/        # Page-level components for routing
│   ├── store/        # Zustand state management files
│   ├── types/        # TypeScript type definitions
│   └── main.tsx      # Application entry point
└── package.json      # Project dependencies and scripts
```

## Contributing
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -m 'Add feature-name'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
