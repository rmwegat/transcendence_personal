# ft_transcendence

# ✅ PHASE 1 — Mandatory Base

## 1. Project Setup

* [ ] Create project root structure
* [ ] Create `/frontend`, `/backend`, `/docker`
* [ ] Initialize Git repository

## 2. SPA Base (TypeScript)

* [ ] Install Vite or esbuild
* [ ] Create `index.html`
* [ ] Create `/frontend/src` structure:

  * [ ] `main.ts`
  * [ ] `router.ts`
  * [ ] `pages/home.ts`
  * [ ] `pages/game.ts`
  * [ ] `pages/tournament.ts`
* [ ] Implement SPA router (pushState + popstate)
* [ ] Ensure Back/Forward buttons work
* [ ] Test in Firefox (latest)

## 3. Local Pong Game

* [ ] Implement GameEngine class
* [ ] Render using `<canvas>`
* [ ] Add paddles, ball, collisions
* [ ] Add 2-player local controls (W/S + Up/Down)
* [ ] Ensure equal paddle speed
* [ ] Add score UI + winner detection

## 4. Tournament System

* [ ] Create alias input page
* [ ] Store players in JS array
* [ ] Auto-generate match order
* [ ] Display upcoming match
* [ ] “Start match” → open Pong game
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

* [ ] Dockerfile for frontend (nginx or Caddy)
* [ ] Dockerfile for backend (Node/Fastify)
* [ ] docker-compose.yml
* [ ] Single command launch: `docker-compose up`
* [ ] Containers:

  * [ ] frontend
  * [ ] backend
  * [ ] nginx reverse proxy

## 7. Reverse Proxy (nginx)

* [ ] Serve SPA (`/`)
* [ ] Proxy `/api` → backend
* [ ] Proxy `/ws` → backend (WebSockets)
* [ ] Configure HTTPS
* [ ] Configure WSS upgrade headers
* [ ] Add security headers:

  * [ ] Content-Security-Policy
  * [ ] X-Frame-Options
  * [ ] X-Content-Type-Options

---

# ✅ PHASE 3 — Core Major Modules (Most Important)

## 8. Backend Framework (Fastify) — Major

* [ ] Initialize Fastify project
* [ ] Add routes:

  * [ ] `/auth/register`
  * [ ] `/auth/login`
  * [ ] `/user/me`
  * [ ] `/user/update`
  * [ ] `/user/avatar`
  * [ ] `/friends/*`
  * [ ] `/matches/*`
* [ ] Input validation (Fastify JSON schema)
* [ ] Global error handler

## 9. Database (SQLite) — Minor

* [ ] Add `database.db`
* [ ] Add migrations:

  * [ ] users
  * [ ] matches
  * [ ] stats
  * [ ] friends
  * [ ] settings
* [ ] Create DB wrapper for prepared statements
* [ ] Test CRUD operations

## 10. Standard User Management — Major

### Backend

* [ ] Register (hashed passwords)
* [ ] Login (session/JWT)
* [ ] Update profile
* [ ] Avatar upload
* [ ] Online/offline tracking
* [ ] Friends system
* [ ] Match history table
* [ ] Protect authenticated routes

### Frontend

* [ ] Registration page
* [ ] Login page
* [ ] Profile page
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
