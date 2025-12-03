# ft_transcendence

# ✅ PHASE 1 — Mandatory Base

## 1. Project Setup

* [x] Create project root structure
* [x] Create `/frontend`, `/backend`, `/docker`
* [x] Initialize Git repository

## 2. SPA Base (TypeScript)

* [x] Install Vite or esbuild
* [x] Create `index.html`
* [x] Create `/frontend/src` structure:

  * [x] `main.ts` (app.ts)
  * [x] `router.ts` (in app.ts)
  * [x] `pages/home.ts` (login.ts)
  * [x] `pages/game.ts` (game_frontend.ts)
  * [x] `pages/tournament.ts` (setup_game.ts)
* [x] Implement SPA router (hash-based routing)
* [x] Multi-view navigation system (/home, /play, /1v1, /game, /profile, /history)
* [x] Ensure Back/Forward buttons work
* [x] Test in Firefox (latest)

## 3. Local Pong Game

* [x] Implement GameEngine class
* [x] Render using `<canvas>`
* [x] Add paddles, ball, collisions
* [x] Add 2-player local controls (W/S + Up/Down)
* [x] Ensure equal paddle speed
* [x] Add score UI + winner detection
* [x] Enhanced visual rendering with gradients and subtle effects
* [x] Professional dark theme styling
* [x] Smooth game animations and effects

## 4. Tournament System

* [x] Create alias input page
* [x] Store players in JS array
* [x] Auto-generate match order
* [ ] Display upcoming match
* [ ] "Start match" → open Pong game
* [ ] Update tournament after each match
* [ ] Display final winner

## 5. Basic Security (Mandatory)

* [ ] Sanitize all user-entered text
* [ ] Output using `.textContent` only
* [ ] Form validation (length, characters)
* [ ] Basic CSP header for local build
* [ ] HTTPS (self-signed) in Docker

---

# ✅ PHASE 2 — Infrastructure Foundation

## 6. Docker Environment

* [x] Dockerfile for frontend (nginx or Caddy)
* [x] Dockerfile for backend (Node/Fastify)
* [x] docker-compose.yml
* [x] Single command launch: `docker-compose up`
* [x] Containers:

  * [x] frontend
  * [x] backend
  * [x] nginx reverse proxy

## 7. Reverse Proxy (nginx)

* [x] Serve SPA (`/`)
* [x] Proxy `/login_service/` → login backend
* [x] Proxy `/game_service/` → game backend
* [x] Service routing working for microservices
* [ ] Proxy `/ws` → backend (WebSockets)
* [ ] Configure HTTPS
* [x] Configure WSS upgrade headers
* [ ] Add security headers:

  * [ ] Content-Security-Policy
  * [ ] X-Frame-Options
  * [ ] X-Content-Type-Options

---

# ✅ PHASE 3 — Core Major Modules (Most Important)

## 8. Backend Framework (Fastify) — Major

* [x] Initialize Fastify project
* [x] Add routes:

  * [x] `/auth/register` (createAccount)
  * [x] `/auth/login` (loginAccount)
  * [x] `/user/me` (auth/me)
  * [ ] `/user/update`
  * [ ] `/user/avatar`
  * [ ] `/friends/*`
  * [ ] `/matches/*`
* [ ] Input validation (Fastify JSON schema)
* [ ] Global error handler

## 9. Database (SQLite) — Minor

* [x] Add `database.db`
* [x] Add migrations:

  * [x] users
  * [x] matches (game_sessions)
  * [ ] stats
  * [ ] friends
  * [ ] settings
* [ ] Create DB wrapper for prepared statements
* [x] Test CRUD operations

## 10. Standard User Management — Major

### Backend

* [x] Register (hashed passwords)
* [x] Login (session/JWT)
* [ ] Update profile
* [ ] Avatar upload
* [ ] Online/offline tracking
* [ ] Friends system
* [x] Match history table
* [x] Protect authenticated routes

### Frontend

* [x] Registration page
* [x] Login page
* [x] Profile page
* [x] 1v1 Match setup page
* [x] Game lobby page
* [x] Enhanced UI with modern dark theme
* [x] Responsive button styling and navigation
* [ ] Friend list
* [ ] Match history UI

---

# ✅ PHASE 4 — Minor Modules

## Minor 1 — Tailwind CSS

* [ ] Install Tailwind
* [ ] Convert existing CSS to utility classes

## Minor 2 — GDPR / Local Data Tools

* [ ] Delete Account
* [ ] Export My Data (JSON)
* [ ] Anonymize Account

## Minor 3 — Game Customization

* [ ] UI panel for game settings:

  * [ ] Ball speed
  * [ ] Paddle size
  * [ ] Powerups toggle
* [ ] Apply settings in local game

## Minor 4 — Multi-language Support

* [ ] Add `/i18n/en.json`, `/i18n/de.json`, `/i18n/fr.json`
* [ ] Add language switcher
* [ ] Replace hardcoded text

## Minor 5 — Support on All Devices

* [ ] Responsive layout using Tailwind
* [ ] Test tablet + mobile

## Minor 6 — Expanding Browser Support

* [ ] Test Chrome or Safari
* [ ] Fix browser-specific issues

## Minor 7 — Accessibility

* [ ] Add ARIA labels
* [ ] Keyboard navigation
* [ ] High-contrast mode
* [ ] Skip-to-content link

## Minor 8 — Stats Dashboard

* [ ] Backend stats endpoint
* [ ] Frontend dashboard (Chart.js or TS-only)
* [ ] Metrics:

  * [ ] Win/loss ratio
  * [ ] Matches played
  * [ ] Average score

---

# ✅ PHASE 5 — Monitoring System (Minor)

→ Combined with Database Minor = **1 Major**

* [ ] Add Prometheus container
* [ ] Add Grafana container
* [ ] Add `/metrics` Fastify plugin
* [ ] Create dashboard:

  * [ ] Backend request rate
  * [ ] Latency
  * [ ] Errors
  * [ ] Uptime

---

# 7 Majors → 100% Achieved

(Now start bonus phase)

---

# ⭐ PHASE 6 — BONUS

## Bonus Major — AI Opponent

* [ ] AI reads game state every 1s
* [ ] AI moves paddle toward ball
* [ ] AI simulates key presses
* [ ] AI uses powerups
* [ ] AI wins sometimes

## Bonus Minor — SSR

* [ ] Add SSR engine to Fastify (EJS/Handlebars)
* [ ] Render landing page server-side
* [ ] Keep SPA intact for internal pages

## Bonus Minor — Additional Accessibility or Language

* [ ] Add one more language OR
* [ ] Add font-size slider for accessibility

---

# 🎯 FINAL COMPLETION TARGETS

* [ ] Mandatory Part PERFECT
* [ ] 7 Majors → 100%
* [ ] Bonus Major (AI) → +10%
* [ ] Bonus Minors (2–3) → +10–15%

✔ **Total: 125%+ achievable**

---

# 🚀 End of TODO file
