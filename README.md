<h1 align="center">Krittin Jaruvisut</h1>
<h3 align="center">Frontend Developer · Thailand</h3>

---

## About me

- Frontend engineer working mostly in Vue, Nuxt, Angular, and Next.js
- I care about UI quality, accessibility, and performance, and about code that stays maintainable
- I design frontend architecture for scale: state management, data flow, component systems, and API integration
- I'm interested in product-minded teams where engineering quality and UX both count

---

## Flagship projects

### [QSpace](https://qspace.fun): multi-tenant queue booking SaaS
Tech: `Next.js 15` `TypeScript` `Supabase`

A multi-tenant queue-booking platform with strict tenant isolation and realtime queue updates.

- Uses Supabase Row-Level Security (RLS) for tenant-safe data access
- Payments default to manual mode: each merchant publishes their own PromptPay or bank details, customers upload a slip, and slip-verification providers check it automatically, so the platform takes no cut. Stripe and Omise are built in but switched off
- Supports phased registration (waitlist, invite, open), staff and resource scheduling, time slots, and add-ons

---

### [Recura](https://recura.fun/): subscription and expense tracker
Tech: `Vue 3` `Vite` `Pinia` `Service Worker`

A finance tracker for subscriptions and recurring expenses, with AI-assisted analysis.

- Connects to AI providers (OpenAI, Gemini, Anthropic, OpenRouter, local models) for spend insights
- Extracts invoice data automatically
- Sends renewal reminders with action buttons and keeps a history of each Keep / Pause / Cancel decision
- Dashboard with monthly and yearly totals, a six-month trend by category, and a calendar view of upcoming charges
- Tracks THB, USD, EUR, and JPY with live exchange rates; data stays in the browser's localStorage, with no backend

---

### [MilkyPlanner](https://milkyplanner.fun): astrophotography planning tool
Tech: `Vanilla JS` `Canvas API` `three.js`

A planning tool for Milky Way photography that computes the sky from a location and time.

- Calculates galactic core position, direction, elevation, moon phase, and the best shooting windows
- Includes an interactive 2D sky-direction map and a 3D sky-dome visualization
- Scans a whole season, night by night, and ranks the nights by shooting conditions
- Works in Thai and English, picking the language from the browser, and shares a plan as a link with location and date

---

### [MeowMap](https://meowmap.fun/): stray cat sighting tracker
Tech: `Next.js 15` `TypeScript` `Neon (PostgreSQL)` `Cloudflare R2` `Leaflet`

A crowdsourced map for reporting and managing stray-cat sightings.

- Shows clustered, status-coded map markers with place search and filters
- Gives every sighting its own shareable link with a preview card, and lets signed-in users post follow-up updates that change its status
- Warns you with a toast when a recent sighting is within 100 m of your location
- Supports email/password and Google/GitHub OAuth sign-in (Neon Auth), optional phone OTP, and admin moderation
- Uploads images straight to R2, with Cloudflare Turnstile for bot protection

---

### [Game Icons Memory](https://game-icons-memory.vercel.app/): icon quiz and memory game
Tech: `Nuxt 3` `TypeScript` `Neon (PostgreSQL)` `Tailwind CSS` `Vitest`

A tech-logo quiz and memory game with a global leaderboard and an admin-managed question catalog.

- Two game modes: a 10-question, 4-choice icon quiz, and memory boards from 3x3 to 6x6
- Shows run time and an answer review after each quiz
- Has auth, user profiles, and an admin panel for question sets, users, and event logs
- Syncs the icon catalog (about 1,400 logos) from upstream sources automatically, with a CI-friendly `--check` mode
- Game logic and server stores are covered by 16 Vitest suites

---

### [ServicePulse](https://servicepulse.fun): uptime and status monitoring SaaS
Tech: `Nuxt 4` `TypeScript` `Express 5` `Neon (PostgreSQL)` `Tailwind CSS`

A full-stack uptime monitoring service with per-user isolation and scheduled health checks.

- JWT auth with HTTP-only cookies, session expiration, and rate limiting
- Per-service check intervals from 1 to 1440 minutes (the Free plan's minimum is 5)
- Webhook notifications on status change, and a filterable, paginated log viewer
- Free, Pro, and Business plans with Stripe billing, and public status pages on the paid plans
- The stack is split into a Nuxt frontend and an Express API, with analytics, billing, and public status-page routes

---

### [Steam Intelligent](https://steam-intelligent.vercel.app/): Steam library and achievement analytics
Tech: `Nuxt 4` `TypeScript` `Nuxt UI v4` `Tailwind CSS v4` `Pinia`

An SSR analytics app that turns a Steam library into playtime and achievement insights.

- Steam OpenID login with encrypted sessions and server-side refresh middleware
- Library, playtime, and achievement data feed dashboard, library, and insights views
- The SteamSpy genre catalog is prebuilt at build time, so nothing is fetched from SteamSpy at request time
- Ships a committed sample library at `/demo`, so the app can be explored without a Steam login
- The API and view layers are covered by more than 50 test files (unit, Nuxt runtime, and e2e)

---

### [Launch Tracker](https://space-x-mu-eight.vercel.app/): orbital launch dashboard
Tech: `Vue 3` `Vite` `Vuetify 3` `Vitest` `Cypress`

A launch dashboard on top of The Space Devs Launch Library 2, covering launches, rockets, crew, spacecraft, pads, and agencies.

- The public API allows about 15 requests per hour, so the app uses a `localStorage` cache (30-minute freshness), de-duplicates in-flight requests, and offers a manual cache-busting refresh
- On HTTP 429 it backs off according to `Retry-After` and falls back to stale cache, so the UI keeps rendering
- 11 routed views with detail pages, with Vitest unit tests on the API service and Cypress set up for e2e

---

### [Pinto Rider Sukhumvit](https://rider-simulation-game.vercel.app): delivery rider simulator
Tech: `Vanilla JS` `three.js` `Vite` `Vitest`

A 3D browser game where you ride a delivery bike through Bangkok, from Silom and Siam out to Thonglor and Ekkamai, on a road graph built from OpenStreetMap centerlines. The UI is in Thai.

- Routes orders with Dijkstra over the road graph, including turn costs, and runs per-road traffic rhythms across shifts
- Two BTS lines run as animated trains on viaducts, with rain and weather effects
- Progression through levels and bike upgrades, with the Silom and Sathorn district locked until level 12
- 22 achievements in five categories (city knowledge, driving, pro play, story, career), such as delivering to every soi in the Asok to Ekkamai area; many pay out cash, unlock rider titles, or award a cosmetic
- Rider cosmetics for the jacket, tiffin carrier, and halo, 14 variants in all, applied live to the 3D rider model
- Needs no backend: the profile lives in `localStorage`, audio is synthesized with WebAudio, and textures are drawn on canvases, so there are no asset files
- Game logic is covered by 16 Vitest test files that run in Node, with no DOM or WebGL

---

### [WebSignal](https://www.websignal.app): SEO, AEO, and GEO audit platform
Tech: `Nuxt 4` `TypeScript` `Neon (PostgreSQL)` `Drizzle` `Playwright` `Chrome MV3` `Vitest`

A platform that audits how visible a website is to search engines and AI answer engines, then tracks the score over time.

- Scores a site against 43 rules across SEO, AEO, and GEO. A plain audit makes no LLM calls; a model is used only on request, with all issues batched into one prompt per audit
- Pins every score to a scoring-profile version, so a history chart moves only when the site changes, not when a rule weight does
- Crawler guards against SSRF by resolving DNS, rejecting private addresses, and pinning the connection to the address it checked, on every redirect hop. It uses Cheerio first and Playwright only when a page needs rendering
- Isolates tenants with Postgres Row Level Security, and the migration fails if the app role could bypass it
- Monorepo where one analyzer rule set runs both on the server and, client-side, in a Chrome extension quick audit
- GEO scores are labelled as heuristic, since they measure what a page exposes to AI crawlers, not whether any engine cites it
- Covered by 90 Vitest test files

---

### [EsportIntel](https://www.esportintel.live): esports matches, teams, and tournaments
Tech: `Nuxt 4` `Nuxt UI v4` `Tailwind CSS v4` `Supabase` `Vitest`

A dashboard for esports data from the PandaScore API, covering leagues, matches, players, teams, tournaments, series, and games.

- Mirrors PandaScore into Supabase on an hourly sync, plus a 5-minute job for live match status, so browsing costs no upstream API requests
- Calls PandaScore only from the server, so the API token never reaches the browser
- Live, schedule, additions, and transfers pages update in place through a Realtime Broadcast signal when a sync lands, with no polling
- Paginated, filterable, sortable lists that keep their filters and page in the URL so they can be shared
- Anonymous Supabase auth backs a per-visitor watchlist that can be upgraded to Google or Discord sign-in, plus a personal feed of upcoming matches for starred teams and players
- Command palette, `.ics` calendar export for fixtures, and a sitemap of about 71k URLs with JSON-LD, `llms.txt`, and an AI-crawler-friendly `robots.txt`
- Covered by 76 Vitest test files

---

## More projects

- [Dealhunt](https://dealhunt.today): game price comparison app (`Vue`, `Nuxt`, `CheapShark API`)
- [Countdown Timer](https://countdown-html.vercel.app/): multi-timer and Pomodoro PWA (`Vanilla JS`, `Web Notifications API`)
- [Easy Bed Management](https://easy-bed-management.vercel.app/): hospital bed/ward tracker with occupancy reporting, no build step (`Vanilla JS`, `CSS Variables`)

---

## Tech stack

### Languages
<p>
  <img src="https://skillicons.dev/icons?i=js,ts,php,swift,html,css" alt="Languages: JavaScript, TypeScript, PHP, Swift, HTML, CSS" />
</p>

### Frameworks and libraries
<p>
  <img src="https://skillicons.dev/icons?i=vue,nuxtjs,vuetify,react,nextjs,tailwind,angular,bootstrap,jquery,laravel,express,fastapi" alt="Frameworks and Libraries" />
</p>

### Backend and databases
<p>
  <img src="https://skillicons.dev/icons?i=nodejs,postgres,firebase,supabase,redis,cloudflare,wordpress" alt="Backend and Databases" />
</p>

### Tools and platforms
<p>
  <img src="https://skillicons.dev/icons?i=git,github,vite,vitest,cypress,figma,aws,vercel,replit,arduino" alt="Tools and Platforms" />
</p>

---

<p align="center">
  <a href="https://holopin.io/@copterdotjs">
    <img src="https://holopin.io/api/user/board?user=copterdotjs" alt="Holopin badges" />
  </a>
</p>
