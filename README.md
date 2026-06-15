# 🎓 CampusAI — IIT Roorkee Unified Campus Intelligence Dashboard

[![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)
[![Node.js](https://img.shields.io/badge/Node.js-Express-green?logo=node.js)](https://nodejs.org/)

> A unified, AI-powered web dashboard designed exclusively for IIT Roorkee students to access essential campus data seamlessly from one central hub.

**🌐 Live Demo:** [https://frontend-ten-theta-33.vercel.app](https://frontend-ten-theta-33.vercel.app)

---

## ✨ Features

- 📚 **Library Catalog** — Search through 18,000+ digital books from Springer, Cambridge, and Wiley with department and material type filters.
- 🍽️ **Canteen Menus** — Browse up-to-date menus and prices for all 21 IITR Bhawan canteens.
- 📅 **Campus Events** — Stay informed about upcoming IITR events (e.g., Cognizance, E-Summit, COMET26) with direct registration links.
- 🎓 **Academic Timetable** — Access department and year-wise schedules complete with professor names and room allocations.
- 🤖 **AI Assistant (CampusAI)** — An interactive chat interface to get instant, context-aware answers about campus facilities, attendance policies, menus, and more.

## 🏗️ Architecture & Tech Stack

The application follows a modern decoupled architecture using the Model Context Protocol (MCP) pattern:

| Layer | Technology | Description |
|-------|------------|-------------|
| **Frontend** | Next.js 14, React, TS, Tailwind CSS | High-performance, responsive user interface |
| **AI Integration** | Claude (Anthropic API) | Natural language understanding for CampusAI |
| **Backend** | Node.js + Express (MCP Servers) | 4 independent microservices managing data |

### MCP Microservices
The backend data is provided by independent services handling specific domains:
- `academics` (Timetables, Courses, & Policies)
- `cafeteria` (Bhawan Menus & Pricing)
- `events` (Fests, Workshops, & Important Dates)
- `library` (Digital Book Catalog)

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/campus-dashboard-main.git
   cd campus-dashboard-main
   ```

2. **Start the Frontend Client**
   ```bash
   cd frontend
   npm install
   npm run dev
   ```
   *The application will be available at `http://localhost:3000`*

3. **Start the MCP Backend Servers**
   In separate terminals, navigate to each server directory inside `mcp-servers/` and run the service:
   ```bash
   cd mcp-servers/<service-name> # (e.g., academics, cafeteria, events, library)
   npm install
   npm start
   ```

## Built by

**Yashasvi** (Enrollment: 24113147) — IIT Roorkee  
*Problem Statement 01 — Unified Campus Intelligence Dashboard with AI Assistant*
