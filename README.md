<div align="center">

# Hi, I'm Mukul Negi 👋

### Java & Spring Boot Backend Developer · Full-Stack Builder

Building APIs, financial systems, and real-time web experiences.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/mukul-negi-927ab325b) [Explore my projects](#-selected-projects) · [What I work with](#-tech-stack) · [Engineering details](#-under-the-hood)

</div>

---

## 👨‍💻 About me

I'm a software developer with experience in **Java, Spring Boot, microservices, SQL Server, React, and TypeScript**. I enjoy connecting reliable backend services with interfaces that feel good to use.

- **Professional experience:** in-house product development at **Fincart Financial Planners**, working on REST APIs, payment and KYC integrations, transaction workflows, webhooks, and SQL operations.
- **Internship:** web development at **DevTown**, using React, Node.js, Express, and MongoDB.
- **Public work:** collaborative coding tools, authenticated notes, data-driven dashboards, and responsive interfaces.
- **Engineering interests:** API design, database performance, real-time synchronization, accessibility, and thoughtful motion.

> My public repositories showcase personal projects. My professional Java/Spring Boot work is described here through my experience.

## 💻 Tech stack

**Backend & APIs**  
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/Express-404d59?style=flat-square&logo=express&logoColor=white) ![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socketdotio&logoColor=white)

**Frontend**  
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwindcss&logoColor=white)

**Data & tools**  
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

---

## 🚀 Selected projects

### [Compile Palace](https://github.com/positron100/compile-palace) · [Live app ↗](https://compile-palace.vercel.app/)

Collaborative code editor with shared rooms, remote cursors, code execution and saved snippets.  
`React` `TypeScript` `Socket.io` `Supabase`

### [CloudBook](https://github.com/positron100/CloudBook) · [Live app ↗](https://cloud-book-frontend-xi.vercel.app/)

JWT-authenticated notes with optimistic updates, search, tags and a tactile writing-desk interface.  
`React` `Express` `MongoDB` `JWT`

### [IPO GMP Desk](https://github.com/positron100/ipo-guru) · [Live app ↗](https://ipo-guru-iota.vercel.app/)

Indian IPO tracker with subscription views, a pluggable data-provider layer and a responsive glass UI.  
`Next.js` `TypeScript` `Tailwind CSS`

### [Portfolio](https://github.com/positron100/portfolio)

Interactive developer portfolio with a 3D companion, architecture maps and project previews.  
`React` `TypeScript` `Three.js`

### [Sattva](https://github.com/positron100/ayurvedic-remedy-suggestor) · [Live app ↗](https://ayurvedic-remedy-suggestor.vercel.app/)

Symptom-based Ayurvedic information tool with deterministic matching, provenance and safety checks.  
`React` `TypeScript` `Vite`

### [TextUtils Enhanced](https://github.com/positron100/TextUtils_enhanced) · [Live app ↗](https://text-utils-enhanced.vercel.app/)

Browser-based text transformations, cleanup, clipboard tools and live counts.  
`React` `JavaScript`

<sub>IPO GMP is unofficial market sentiment, not investment advice. Sattva provides general information, not medical advice.</sub>

---

## 🔎 Under the hood

**Expand a project to explore the engineering behind it.**

<details>
<summary><b>Compile Palace — collaboration and code execution</b></summary>

<br>

- **Stack:** React, TypeScript, CodeMirror 5, Socket.io, Express, and Supabase.
- Shared rooms synchronize code, participant presence, and remote cursor positions.
- Judge0 handles execution, with a JDoodle fallback through a Supabase Edge Function.
- Supabase provides authentication and a per-user snippet library.
- **Tradeoff:** synchronization uses whole-document snapshots with last-write-wins semantics; simultaneous edits can overwrite each other.

[Frontend](https://github.com/positron100/compile-palace) · [Realtime backend](https://github.com/positron100/code-editor-)

</details>

<details>
<summary><b>CloudBook — full-stack notes and optimistic updates</b></summary>

<br>

- **Stack:** React, TypeScript, Express, MongoDB, Mongoose, and JWT.
- A workspace monorepo shares typed contracts between frontend and backend.
- Note changes appear immediately, then reconcile with the server.
- Search, tag filters, and sorting sit alongside keyboard access and reduced-motion support.

[Read the architecture and API overview](https://github.com/positron100/CloudBook#readme)

</details>

<details>
<summary><b>IPO GMP Desk — provider boundaries and honest data states</b></summary>

<br>

- **Stack:** Next.js, React, TypeScript, and Tailwind CSS.
- Pages use a service layer rather than calling external providers directly.
- Provider validation and ISR caching support listing, detail, and subscription views.
- Missing values appear as unavailable instead of being silently converted to zero.
- Responsive layouts, reduced-motion support, and per-page SEO are part of the implementation.

[Explore the implementation](https://github.com/positron100/ipo-guru#readme)

</details>

<details>
<summary><b>Portfolio & Sattva — interaction design with clear constraints</b></summary>

<br>

- **Portfolio:** React and TypeScript with a lazy-loaded 3D companion, shared motion tokens, keyboard-accessible controls, and light/dark themes.
- **Sattva:** a pure TypeScript recommendation engine with curated knowledge, source provenance, and red-flag handling.
- Sattva's optional LLM layer is limited to input interpretation and presentation; it cannot select remedies or override safety rules.

[Portfolio](https://github.com/positron100/portfolio#readme) · [Sattva](https://github.com/positron100/ayurvedic-remedy-suggestor#readme)

</details>

---

## 📊 GitHub activity

<div align="center">

<img src="https://github-readme-stats.shion.dev/api?username=positron100&theme=tokyonight&hide_border=true&include_all_commits=false&count_private=false" alt="Mukul Negi's public GitHub statistics" width="480" />

<br>

<img src="https://streak-stats.demolab.com/?user=positron100&theme=tokyonight&hide_border=true" alt="Mukul Negi's GitHub contribution streak" width="480" />

<br>

<img src="https://github-readme-stats.shion.dev/api/top-langs/?username=positron100&theme=tokyonight&hide_border=true&layout=compact" alt="Languages represented in Mukul Negi's public GitHub repositories" width="400" />

</div>

<sub>Cards are provided by third-party services and may be temporarily unavailable. Repository language statistics describe public code, not my complete professional skill set.</sub>

---

## 🤝 Let's connect

Interested in Java backend development, API integrations, or real-time web applications? I'd be happy to talk.

**[LinkedIn](https://www.linkedin.com/in/mukul-negi-927ab325b)** · **[All public repositories](https://github.com/positron100?tab=repositories&type=public)**

---

<div align="center">
<sub>Built with <a href="https://gprm.itsvg.in/">GPRM</a> and customized around my work.</sub>
</div>
