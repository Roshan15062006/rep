TrustNet AI — Intelligent Zero-Trust Security Platform
TrustNet AI is an interactive cybersecurity monitoring and incident-intelligence platform designed to help organizations detect, understand, and respond to suspicious user, device, and network behavior. The project combines a React/Vite frontend, a FastAPI backend, machine-learning-assisted risk scoring, a device registry, behavioral analytics, incident correlation, response agents, and a live security dashboard.

The platform follows a zero-trust security model: every user, device, request, and session must continuously demonstrate trust instead of being automatically accepted because it is inside a network perimeter.

Project Purpose
Traditional security dashboards often generate large numbers of disconnected alerts. Security teams must manually determine whether an event is meaningful, how severe it is, what assets may be affected, and what response should be taken.

TrustNet AI addresses this problem by correlating multiple signals into a single security view. The system analyzes:

User behavior
Device fingerprints
Login history
Network activity
Geographic patterns
Request behavior
Asset criticality
Risk propagation paths
Incident history
Authentication and MFA events
The objective is to provide security operators with an explainable view of what happened, why it matters, and which response should be considered.

Main Features
Interactive Security Dashboard
The authenticated dashboard provides a centralized security command center with:

Average user-risk scoring
Active incident counts
Trusted and untrusted device counts
Network anomaly metrics
Recent incident summaries
Live network topology
Device registry information
WebSocket connection status
Attack simulation controls
Notification indicators
Admin controls based on user permissions
The dashboard is designed with a dark red-and-black security theme, animated transitions, responsive layouts, glowing status indicators, and visual risk badges.

Public Interactive Demo
The project includes a public interactive preview at:

Copy code block
/demo
This preview can be used without connecting the backend. It allows users to experience the interface before configuring authentication or backend services.

The demo includes:

System risk metrics
Active signal counts
Protected asset metrics
Response SLA information
Interactive security graph visualization
Attack-chain simulation
Signal stream tab
Response plan tab
Analyst approval interaction
Activity feed
Baseline and critical-state views
The simulated attack interaction changes the security state, increases the risk score, displays additional alerts, updates the activity feed, and presents a recommended response path.

Command Center Navigation
The dashboard includes an interactive Command Center. Users can open it by clicking the Command Center button or pressing:

Copy code block
Ctrl + K
The command center provides searchable navigation to:

Overview
Behavior Analytics
Network Activity
Risk Propagation
Incident Center
Admin Panel
Keyboard navigation is supported with:

Arrow Up
Arrow Down
Enter
Escape
This allows security operators to move quickly between important areas of the platform.

Application Architecture
TrustNet AI is divided into frontend and backend layers.

Frontend
The frontend is built using:

React
TypeScript
Vite
React Router
Tailwind CSS
Radix UI components
Framer Motion
Lucide icons
Recharts
Three.js
Vitest
The frontend source code is located in:

Copy code block
trustnet_all/src/
Important frontend areas include:

Copy code block
src/App.tsx
src/components/
src/pages/
src/services/
src/store/
src/hooks/
src/data/
src/styles/
Backend
The backend is built using:

Python
FastAPI
SQLite
WebSocket communication
Authentication and authorization services
Machine-learning modules
Incident and audit models
Agent orchestration
The backend source code is located in:
