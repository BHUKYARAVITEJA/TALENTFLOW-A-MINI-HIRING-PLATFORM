# TALENTFLOW-A-MINI-HIRING-PLATFORM
TalentFlow is a comprehensive front-end React application designed as a mini hiring platform for HR teams. This is a frontend-only implementation that uses Mock Service Worker (MSW) to simulate a backend API and IndexedDB (via Dexie) for local data persistence
## Key Features
1. Jobs Board Management - Create, edit, archive, and reorder job postings with drag-and-drop functionality
2. Candidate Management - Track 1000+ candidates through hiring stages using a Kanban board interface
3. Assessment Builder - Create dynamic, multi-section assessments with conditional logic and live preview
## Technical Architecture
<img width="2400" height="1600" alt="image" src="https://github.com/user-attachments/assets/9ea7f167-c8ad-4284-9509-1344fe8f0543" />
## Frontend Core
1. React 18+ with TypeScript for type safety
2. Vite as the build tool for fast development
3. React Router DOM for client-side routing
4. Tailwind CSS for utility-first styling
## State Management
1. Redux Toolkit with separate slices for Jobs, Candidates, and Assessments
2. Redux Thunks for async operations
3. Optimistic updates with rollback support
## Data Layer
1. Dexie.js (IndexedDB wrapper) for local persistence
2. MSW (Mock Service Worker) for API simulation
3. Axios as HTTP client
## UI Components
1. Radix UI for accessible component primitives
2. Lucide React for icons
3. React Hot Toast for notifications
## Architecture Pattern
This application follows a layered architecture:
┌─────────────────────────────────────────┐
│ React Components (UI)               │
├─────────────────────────────────────────┤
│ Redux Store (State Management)      │
├─────────────────────────────────────────┤
│ Axios API Client (HTTP)             │
├─────────────────────────────────────────┤
│ MSW Handlers (Mock API Layer)       │
├─────────────────────────────────────────┤
│ Dexie/IndexedDB (Persistence Layer) │
└─────────────────────────────────────────┘

