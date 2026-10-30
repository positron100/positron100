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

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white) ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) ![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB) ![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101) ![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) ![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white) ![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

| Area | What I work with |
| --- | --- |
| Backend | Java, Spring Boot, REST APIs, microservices, Node.js, Express |
| Data | SQL Server, T-SQL, stored procedures, MongoDB, Mongoose |
| Frontend | React, TypeScript, JavaScript, Next.js, HTML, CSS, Tailwind CSS |
| Real-time | Socket.io, room-based synchronization, presence, remote cursors |
| Tools & delivery | Git, GitHub, Postman, Vercel, Render |

## 🚀 Selected projects

| Project | What it does | Explore |
| --- | --- | --- |
| **Compile Palace** | Collaborative code editor with shared rooms, remote cursors, code execution, and saved snippets. | [Source](https://github.com/positron100/compile-palace) · [Live app](https://compile-palace.vercel.app/) |
| **CloudBook** | JWT-authenticated notes with optimistic updates, search, tags, and a tactile writing-desk interface. | [Source](https://github.com/positron100/CloudBook) · [Live app](https://cloud-book-frontend-xi.vercel.app/) |
| **IPO GMP Desk** | Indian IPO tracker with subscription views, a pluggable data-provider layer, caching, and a responsive glass UI. | [Source](https://github.com/positron100/ipo-guru) · [Live app](https://ipo-guru-iota.vercel.app/) |
| **Portfolio** | Interactive developer portfolio with a 3D companion, architecture maps, theme transitions, and project previews. | [Source & overview](https://github.com/positron100/portfolio) |
| **Sattva** | Symptom-based Ayurvedic information tool with deterministic matching, provenance, and explicit safety checks. | [Source](https://github.com/positron100/ayurvedic-remedy-suggestor) · [Live app](https://ayurvedic-remedy-suggestor.vercel.app/) |
| **TextUtils Enhanced** | Browser-based text transformations, cleanup, clipboard tools, and live text counts. | [Source](https://github.com/positron100/TextUtils_enhanced) · [Live app](https://text-utils-enhanced.vercel.app/) |

<sub>IPO GMP is unofficial market sentiment, not investment advice. Sattva provides general information, not medical advice.</sub>

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

## 📊 GitHub activity

<div align="center">

<img src="https://github-readme-stats.shion.dev/api?username=positron100&theme=tokyonight&hide_border=true&include_all_commits=false&count_private=false" alt="Mukul Negi's public GitHub statistics" width="480" />

<br>

<img src="https://streak-stats.demolab.com/?user=positron100&theme=tokyonight&hide_border=true" alt="Mukul Negi's GitHub contribution streak" width="480" />

<br>

<img src="https://github-readme-stats.shion.dev/api/top-langs/?username=positron100&theme=tokyonight&hide_border=true&layout=compact" alt="Languages represented in Mukul Negi's public GitHub repositories" width="400" />

</div>

<sub>Cards are provided by third-party services and may be temporarily unavailable. Repository language statistics describe public code, not my complete professional skill set.</sub>

## 🤝 Let's connect

Interested in Java backend development, API integrations, or real-time web applications? I'd be happy to talk.

**[LinkedIn](https://www.linkedin.com/in/mukul-negi-927ab325b)** · **[All public repositories](https://github.com/positron100?tab=repositories&type=public)**

---

<div align="center">
<sub>Built with <a href="https://gprm.itsvg.in/">GPRM</a> and customized around my work.</sub>
</div>
