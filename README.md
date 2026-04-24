<div align="center">

# EcoAlmaty

**AI-powered eco-education app for students in Almaty, Kazakhstan**

[![Live Demo](https://img.shields.io/badge/Live_Demo-GitHub_Pages-2ea44f?style=for-the-badge&logo=github)](https://imanss-ai.github.io/EcoAlmaty)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)
[![Built With](https://img.shields.io/badge/Built_With-React_18-61DAFB?style=for-the-badge&logo=react)](https://react.dev)

<br/>

<img src="https://img.shields.io/badge/Hackathon_Project-2026-ff6b35?style=flat-square" alt="Hackathon 2026"/>

---

*EcoAlmaty turns real-time air quality data into daily micro-lessons, challenges, and community competition — making environmental awareness a habit, not a chore.*

</div>

<br/>

## The Problem

Almaty consistently ranks among the most polluted cities in Central Asia. The Zailiysky Alatau mountains trap pollutants in a natural bowl, causing dangerous smog — especially in winter when thousands of homes burn coal for heating. Yet most residents, especially students, have no daily touchpoint with air quality data or actionable ways to reduce their footprint.

## Our Solution

EcoAlmaty is a mobile-first app that:

- **Shows live AQI data** from Almaty's monitoring stations in a way that's immediately understandable (emoji reactions, plain language, color-coded districts)
- **Teaches something new every day** through AI-generated micro-lessons about local environmental issues
- **Gamifies eco-habits** with streaks, badges, eco scores, and a class leaderboard
- **Makes it actionable** with daily tips tied to current air conditions

## Features

| Screen | Description |
|--------|-------------|
| **Dashboard** | Live AQI with emoji reactions, swipeable lesson cards, actionable daily tips, eco score ring |
| **Map** | Interactive SVG map of Almaty districts with color-coded AQI per zone |
| **Challenge** | Daily 3-question quiz about local air quality and ecology |
| **Friends** | Class leaderboard with podium, score deltas, and friendly competition |
| **Profile** | Score breakdown, weekly activity chart, badge collection, dark/light mode |
| **Onboarding** | 5-step lifestyle quiz (commute, diet, waste, energy, transport) to personalize the experience |
| **Notifications** | AQI alerts, streak reminders, badge unlocks, friend updates |

## Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | React 18, JSX (Babel in-browser) |
| **Styling** | CSS-in-JS, CSS Animations, SVG graphics |
| **Typography** | DM Serif Display (editorial headings), Plus Jakarta Sans (UI) |
| **Device Frame** | Custom iOS 26 Liquid Glass frame component |
| **Data** | Simulated AQI with real Almaty district mapping |
| **Persistence** | localStorage for user state, onboarding, preferences |

## Architecture (Production Roadmap)

```
┌──────────────┐     ┌──────────────┐     ┌──────────────────┐
│   iOS App    │────>│   Backend    │────>│  AQI Data APIs   │
│  (SwiftUI)   │     │  (FastAPI)   │     │  (AirVisual,     │
│              │     │              │     │   OpenWeather)    │
└──────────────┘     └──────┬───────┘     └──────────────────┘
                            │
                     ┌──────┴───────┐
                     │   AI Layer   │
                     │ (Claude API) │
                     │  - Lessons   │
                     │  - Tips      │
                     │  - Quizzes   │
                     └──────────────┘
```

**Production stack:**
- **Mobile:** SwiftUI (iOS) with MVVM architecture
- **Backend:** FastAPI + PostgreSQL
- **AI:** Claude API for daily lesson generation, personalized tips, and quiz creation
- **Data:** IQAir / OpenWeather AQI APIs for real-time Almaty station data
- **Auth:** Apple Sign In + school email verification

## Quick Start

No build step required. Just open in a browser:

```bash
# Clone the repo
git clone https://github.com/IManss-ai/EcoAlmaty.git

# Open the app
open EcoAlmaty/index.html
```

Or visit the **[Live Demo](https://imanss-ai.github.io/EcoAlmaty)**.

### Interactive Controls

- **AQI Slider** (top bar) — drag to simulate different air quality levels and watch the entire app react
- **Onboarding** — completes on first visit, restart via Tweaks panel
- **Dark/Light mode** — toggle in Profile screen

## Target Users

- **Primary:** University and high school students in Almaty (ages 16-24)
- **Secondary:** Eco-conscious young professionals
- **Tertiary:** Schools and universities (bulk adoption for environmental curriculum)

## Business Model

| Revenue Stream | Description |
|----------------|-------------|
| **B2B School Licenses** | Per-student annual subscription for schools integrating EcoAlmaty into curriculum |
| **Municipal Partnerships** | Almaty city government sponsorship for citizen engagement |
| **Sponsored Challenges** | Local eco-brands sponsor daily challenges and reward redemptions |
| **Premium Insights** | Detailed personal carbon footprint analytics for power users |

## Why Almaty?

- **Geographic advantage:** Mountain bowl geography = persistent air quality problem = daily relevance
- **Regulatory tailwind:** Kazakhstan's Green Economy initiative and Almaty 2050 sustainability targets
- **Untapped market:** No local competitor combines AQI data + education + gamification in Kazakh/Russian
- **Scale path:** Model replicable to Astana, Bishkek, Tashkent, and other Central Asian cities

## Team

Built by students from Almaty, Kazakhstan.

## License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**[Live Demo](https://imanss-ai.github.io/EcoAlmaty)** · **[Report Bug](https://github.com/IManss-ai/EcoAlmaty/issues)**

</div>
