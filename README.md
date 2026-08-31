<h1 align="center">Krittin Jaruvisut</h1>
<h3 align="center">Frontend Developer · Thailand 🇹🇭</h3>

---

## 🚀 About Me

- Frontend-focused engineer with strong experience in **Vue**, **Nuxt**, **Angular**, and **Next.js**
- I care deeply about **UI quality**, **accessibility**, **performance**, and long-term maintainability
- Comfortable designing frontend architecture for scale: state management, data flow, component systems, and API integration
- Interested in product-minded teams where engineering quality and UX both matter

---

## 🌟 Flagship Projects

### [QSpace](https://qspace-app.vercel.app/) — Multi-Tenant Queue Booking SaaS
**Tech:** `Next.js 14` `TypeScript` `Supabase`

Built a multi-tenant queue-booking platform with strict tenant isolation and realtime queue updates.

- Implemented **Supabase Row-Level Security (RLS)** for tenant-safe data access
- Designed provider-agnostic payment layer for **PromptPay/bank transfer**, **Stripe**, and **Omise**
- Added phased registration (waitlist/invite/open), staff/resource scheduling, time slots, and add-ons

> Impact: Add concrete metrics here (e.g., active tenants, p95 latency, onboarding time reduction)

---

### [Recura](https://recura.fun/) — Subscription & Expense Tracker
**Tech:** `Vue 3` `Vite` `Pinia` `Service Worker`

Built a finance tracker for subscriptions and recurring expenses with AI-assisted analysis.

- Integrated AI providers (OpenAI, Gemini, Anthropic, OpenRouter, local models) for spend insights
- Added automatic invoice extraction and decision workflows (**Keep / Pause / Cancel**)
- Implemented multi-currency tracking with live exchange rates and renewal reminders

> Impact: Add measurable outcomes (e.g., monthly active users, retention, notification engagement)

---

### [MilkyPlanner](https://milkyplanner.fun) — Astrophotography Planning Tool
**Tech:** `Vanilla JS` `Canvas API` `three.js`

Created a planning tool for Milky Way photography with location/time-based sky computation.

- Calculates galactic core position, direction, elevation, moon phase, and best shooting windows
- Built interactive **2D sky-direction map** and **3D sky-dome visualization**
- Added multi-night season scan ranked by shooting conditions

> Impact: Add usage/performance metrics if available

---

### [MeowMap](https://meowmap.fun/) — Stray Cat Sighting Tracker
**Tech:** `Next.js 15` `TypeScript` `Neon (PostgreSQL)` `Cloudflare R2` `Leaflet`

Developed a crowdsourced map for reporting and managing stray-cat sightings.

- Clustered, status-coded map markers with location-based filtering
- Implemented auth (email/password + Google/GitHub OAuth) and admin moderation
- Built direct-to-R2 image upload flow with **Cloudflare Turnstile** bot protection

> Impact: Add community and moderation metrics

---

### [Game Icons Memory](https://game-icons-memory.vercel.app/) — Icon Quiz & Memory Game
**Tech:** `Nuxt 3` `TypeScript` `Neon (PostgreSQL)` `Tailwind CSS` `Vitest`

Built a tech-logo quiz and memory game backed by a global leaderboard and an admin-managed question catalog.

- Two game modes: 10-question 4-choice icon quiz and memory boards from **3x3 to 6x6**
- Added auth, user profiles, and an admin panel for question sets, users, and event logs
- Automated icon-catalog sync (~1,400 logos) from upstream sources with a CI-friendly `--check` mode
- Covered game logic and server stores with **16 Vitest suites**

> Impact: Add engagement metrics here (e.g., runs played, leaderboard submissions, returning players)

---

### [ServicePulse](https://servicepulse.fun) — Uptime & Status Monitoring SaaS
**Tech:** `Nuxt 4` `TypeScript` `Express 5` `Neon (PostgreSQL)` `Tailwind CSS`

Built a full-stack uptime monitoring service with per-user isolation and scheduled health checks.

- Implemented **JWT auth** with HTTP-only cookies, session expiration, and rate limiting
- Added **multi-region checks from 4 regions** with per-service intervals (1–1440 min)
- Built webhook notifications on status change plus a filterable, paginated log viewer
- Split the stack into a Nuxt frontend and an Express API with analytics, billing, and public status-page routes

> Impact: Add operational metrics here (e.g., monitored endpoints, checks/day, alert delivery latency)

---

### [Steam Intelligent](https://steam-intelligent.vercel.app/) — Steam Library & Achievement Analytics
**Tech:** `Nuxt 4` `TypeScript` `Nuxt UI v4` `Tailwind CSS v4` `Pinia`

Built an SSR analytics app that turns a Steam library into playtime and achievement insights.

- Implemented **Steam OpenID login** with encrypted sessions and server-side refresh middleware
- Aggregated library, playtime, and achievement data into dashboard, library, and insights views
- Prebuilt the SteamSpy genre catalog at build time so **nothing is fetched from SteamSpy at request time**
- Covered the API and view layers with **28 Vitest suites** (unit + Nuxt runtime)

> Impact: Add usage metrics here (e.g., linked Steam accounts, libraries analyzed, cache hit rate)

---

### [Launch Tracker](https://space-x-mu-eight.vercel.app/) — Orbital Launch Dashboard
**Tech:** `Vue 3` `Vite` `Vuetify 3` `Cypress`

Built a launch dashboard over **The Space Devs Launch Library 2** covering launches, rockets, crew, spacecraft, pads, and agencies.

- Designed a caching layer around a **~15 requests/hour** public API: `localStorage` cache, in-flight request de-duplication, and a manual cache-busting refresh
- Handled **HTTP 429** with `Retry-After`-aware backoff and stale-cache fallback so the UI keeps rendering
- Built 11 routed views with detail pages and end-to-end coverage in Cypress

> Impact: Add usage metrics here (e.g., sessions, cache hit rate, API calls saved)

---

## 🧪 More Projects

- [Dealhunt](https://dealhunt.today) — Game price comparison app (`Vue`, `Nuxt`, `CheapShark API`)
- [Countdown Timer](https://countdown-html.vercel.app/) — Multi-timer and Pomodoro PWA (`Vanilla JS`, `Web Notifications API`)
- [Easy Bed Management](https://easy-bed-management.vercel.app/) — Hospital bed/ward tracker with occupancy reporting, no build step (`Vanilla JS`, `CSS Variables`)

---

## 🛠️ Tech Stack

### Languages
<p>
  <img src="https://skillicons.dev/icons?i=js,php,swift,html,css" alt="Languages: JavaScript, PHP, Swift, HTML, CSS" />
</p>

### Frameworks & Libraries
<p>
  <img src="https://skillicons.dev/icons?i=vue,nuxtjs,vuetify,angular,bootstrap,jquery,laravel,express,fastapi" alt="Frameworks and Libraries" />
</p>

### Backend & Databases
<p>
  <img src="https://skillicons.dev/icons?i=nodejs,firebase,supabase,redis,wordpress" alt="Backend and Databases" />
</p>

### Tools & Platforms
<p>
  <img src="https://skillicons.dev/icons?i=git,github,vite,cypress,figma,aws,vercel,replit,arduino" alt="Tools and Platforms" />
</p>

---

## 📈 Engineering Highlights

- Designed and shipped **multi-tenant frontend/backend flows** with strict data boundaries
- Built production-ready integrations for **payments, auth, file upload, and realtime updates**
- Focused on clean architecture and maintainability for feature-heavy frontend products

---

<p align="center">
  <a href="https://holopin.io/@copterdotjs">
    <img src="https://holopin.io/api/user/board?user=copterdotjs" alt="Holopin badges" />
  </a>
</p>
