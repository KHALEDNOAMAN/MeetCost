# MeetCost
Real-time Meeting Cost Calculator PWA

Companies waste $37B/year on unnecessary meetings.

## Deploy
Deploy to Vercel.

## Overview
MeetCost is a Real-time Meeting Cost Calculator Progressive Web App (PWA). It shows how much a meeting costs as it happens, with fun messages at thresholds.

## Features
- Real-time animated counter
- Multi-currency support
- Fun messages at $50, $200, $500, $1000 thresholds
- Meeting summary with share functionality
- PWA installable

## Architecture
React Single Page Application (SPA) with component state management. No backend needed.

## Tech Stack
React, TypeScript, Tailwind CSS, Framer Motion, Vite

## How It Works
User sets attendees and hourly rate -> Timer starts -> Cost is calculated as (attendees * rate / 3600) * elapsed_seconds -> Animated display shows the cost ticking up.

## Screenshots/Demo
`	ext
================================
       Meeting Cost
        $ 520.45
  "Time is money, literally!"
================================
`

## Installation
`ash
git clone <repo-url>
cd MeetCost
npm install
npm run dev
`

## Usage
Open your browser, set the number of attendees and the average hourly rate, click Start, and watch the cost tick up.

## Project Structure
`	ext
src/
â”œâ”€â”€ App.tsx
â”œâ”€â”€ components/
â”‚   â”œâ”€â”€ SetupForm.tsx
â”‚   â”œâ”€â”€ CostCounter.tsx
â”‚   â”œâ”€â”€ Summary.tsx
â”‚   â””â”€â”€ CurrencyDisplay.tsx
â””â”€â”€ lib/
    â”œâ”€â”€ calculator.ts
    â””â”€â”€ messages.ts
`

## Future Improvements/Roadmap
- Slack integration
- Calendar sync
- Team cost reports
- Historical data
- Dark/light themes
