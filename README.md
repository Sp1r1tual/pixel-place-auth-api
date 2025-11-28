# 🎨 Pixel Place (Api)

**Pixel Place** is an interactive online platform where users collaborate to create a massive pixel canvas — one pixel at a time. Inspired by projects like Reddit r/place, w/place, and other collective art experiments, it turns chaos and creativity into a living digital mosaic.

---

## 💡 Concept

**Pixel Place isn’t just a project — it’s a social experiment.** It’s about coexistence on a single canvas, where hundreds of users shape a shared digital world — sometimes chaotic, sometimes beautiful, always alive.

It’s pixel democracy: **each user gets one pixel, but together, they build art.**

---

## 🚀 Features

- 🧱 Live collaborative canvas — see others’ updates instantly via WebSockets
- 🔐 JWT authentication with refresh tokens
- 🎨 Color palette — choose from a curated set of colors
- 🔋 Energy system — each pixel placement consumes energy that regenerates over time
- 👩‍🦰 User profiles — displaying statistics and users avatars
- 🪙 Shop — users have the ability to purchase upgrades with in-game currency

---

## 🛠️ Tech Stack

- **Runtime:** Node.js
- **Framework:** Express
- **Language:** TypeScript
- **Realtime Engine:** Socket.IO
- **Database Layer:** Supabase (PostgreSQL)
- **Authentication:** JSON Web Tokens
- **Validation:** express-validator
- **Security:** bcrypt, cookie-parser, CORS, dotenv
- **Tooling:** ESLint, Prettier, Husky, lint-staged

📐 **Architecture**: Client ↔ Server ↔ MailService ↔ Database

---

## ⚠️ There is currently a problem with registration for Apple products

At the moment, users on Apple devices may encounter issues during the registration process. This limitation is caused by the way JWT tokens interact with cookies when a project operates across multiple domains. Due to current hosting constraints, the application cannot be deployed on a single shared domain, and as a result, Apple’s security restrictions prevent cookies from being stored or read reliably during authentication.

The registration itself is completed successfully, but the refresh mechanism does not function as expected. Because the refresh token cannot be properly saved or accessed in the browser, sessions on Apple devices expire without the ability to renew them automatically.

---

## 🌐 Future Plans

- 🏆 Leaderboard system — global ranking based on activity, precision, and contribution streaks; highlights top creators and pixel warriors.

- 🎁 Daily bonuses & streak rewards — log in daily to earn cooldown reductions, cosmetic effects, or limited-time colors.

- 🧱 Moderation tools — community-driven reporting and restoration systems to prevent vandalism and maintain fair play.

- 🪄 Seasonal events & limited challenges — themed canvases, world resets, or time-limited events that bring the community together in bursts of creativity.

- ⚡ And much more!

---

## 📜 License

MIT © 2025 — built with ❤️ by the Pixel Place community
