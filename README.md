<div align="center">
<img src="assets/banner.svg" alt="Abhay: full-stack and DevOps engineer. Products: Kenora, LibraryLogix, Failover." width="100%">

<br/>

[![Profile views](https://komarev.com/ghpvc/?username=abhay112&color=6366f1&style=flat-square&label=profile+views)](https://github.com/abhay112)
&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhay-kumar-verma-a27a17240/)
&nbsp;
[![GitHub followers](https://img.shields.io/github/followers/abhay112?style=flat-square&color=6366f1&label=followers)](https://github.com/abhay112?tab=followers)

</div>

<br>

I design, build and run software end to end: React front ends, TypeScript, Go and Node back ends, the data underneath, and the infrastructure and monitoring it all runs on. These are the products I'm running.

---

## Products

<a href="https://valuedefine.com/login"><img src="assets/kenora.svg" alt="Valuedefine: geospatial analytics" width="100%"></a>

**ValueDefine** is a geospatial analytics platform. Bring your data in, shape it with visual workflows, build interactive maps with widgets, and share them by link.

- **Visual workflows.** A node editor on top of a DuckDB workflow engine turns raw datasets into map-ready layers.
- **Interactive maps.** Vector tiles, widgets and shareable links.
- **Market Insights.** Describe your datasets, pick levels and measures, and get KPI cards, rankings, trends and tiles.
- **Built with** React 19, TypeScript, Vite, MapLibre GL, React Flow and TanStack Query on the front; a Go API and tile service plus a Node/TypeScript workflow engine behind it; PostgreSQL with PostGIS for data.

**[Open ValueDefine](https://valuedefine.com/login)** (sign-in required)

<details>
<summary>How it fits together</summary>

```mermaid
flowchart LR
Web["React app<br/>MapLibre + React Flow"] --> API["Go API"]
Web --> Tiles["Go tile service"]
API --> Engine["Workflow engine<br/>Node + DuckDB"]
API --> DB[("PostgreSQL<br/>+ PostGIS")]
Tiles --> DB
Engine --> DB
```

</details>

<br>

<a href="https://library-logix-frontend-react-admin.vercel.app/"><img src="assets/library-logix.svg" alt="LibraryLogix: library management" width="100%"></a>

**LibraryLogix** replaces paper registers and guesswork in study libraries with one system for seats, shifts, attendance and fees, for the people who run the library and the students who use it.

- **Admin dashboard.** Student profiles, morning, evening and full-day shifts, fee status and renewals, and live attendance.
- **Seat designer.** Draw a library floor plan with drag and drop, then see every seat as free, taken, reserved or locked.
- **Student portal.** Students check their attendance, assigned seat and fee status, and request a seat for an admin to approve.
- **Built with** a Turborepo monorepo (admin app, seat designer, shared auth) in React 18, Vite, Tailwind CSS 4, Radix and shadcn/ui, Redux Toolkit and Recharts; a NestJS and Fastify API on MongoDB with Swagger docs, JWT auth, Docker and Nginx, and Prometheus, Grafana and Loki for monitoring.

**[Open the admin app](https://library-logix-frontend-react-admin.vercel.app/)**

<details>
<summary>How it fits together</summary>

```mermaid
flowchart LR
Designer["Seat designer"] --> Admin["Admin app"]
Admin --> API["NestJS + Fastify API"]
Student["Student portal"] --> API
API --> Mongo[("MongoDB")]
API -. metrics and logs .-> Obs["Prometheus · Grafana · Loki"]
```

</details>

<br>

<a href="https://failover.vikalpshorthand.com/"><img src="assets/failover.svg" alt="Failover: learn system design by breaking it" width="100%"></a>

**Failover** teaches system design by letting you build the system and then break it. You drag servers, caches, queues and databases onto a canvas, push load through the design, and watch which part gives way.

- **Content.** 38 modules and 256 lessons, from "what is system design" to replication, partitioning and global availability.
- **Hands-on labs.** 64 labs across classic systems (chat, feeds, ride hailing, payments) and cloud designs, each with an API step, a data-model step, rising load, a monthly budget and incidents such as a lost node or a cold cache.
- **A simulator you can trust.** A deterministic capacity and cost model with 33 component types. Every lab's reference answer is proven solvable by the same engine, and 560+ automated tests keep it honest.
- **AI systems track.** 14 modules and 18 labs on LLM gateways, retrieval, agents, evaluation, safety and serving models at scale.
- **Built with** Next.js 15, React 19, TypeScript, Tailwind CSS 4 and Zod, deployed on Vercel. Progress is saved in your browser, so there is nothing to sign up for.

**[Open Failover](https://failover.vikalpshorthand.com/)**

<br>

---

## More I've built

| Project | What it is |
| --- | --- |
| [**Car Fight**](https://github.com/abhay112/Cubicle_Crash) | A local multiplayer car battle game. Every player's webcam photo goes on the roof of their car, then everyone fights in one arena with random power-ups. |
| [**Content Aggregator**](https://github.com/abhay112/content-aggregator-backend-service) · [demo](https://content-aggregator-frontend-azure.vercel.app) | A Node, Express and TypeScript service that pulls technical content from Hacker News, Dev.to, Reddit and Lobsters into one searchable feed, refreshed by background jobs. |
| [**React Performance Demos**](https://github.com/abhay112/performanceTechniques) · [demo](https://performance-techniques.vercel.app) | Seven interactive demos of real React performance problems: how to spot each one, measure it and fix it. |
| [**Centralized Monitoring Stack**](https://github.com/abhay112/centralizedMonitoring) | A Dockerized Prometheus, Loki and Grafana stack that watches several PM2 and Docker services from one place. |
| [**MERN on Kubernetes**](https://github.com/abhay112/mern-docker) | A full-stack CRUD app (Next.js, Express, MongoDB) packaged with Docker and run on Kubernetes. |

---

## Toolbox

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Linux](https://img.shields.io/badge/Linux_VPS-FCC624?style=flat-square&logo=linux&logoColor=black)

---

<div align="center">

[![GitHub stats](https://github-readme-stats.vercel.app/api?username=abhay112&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=6366f1&icon_color=6366f1&text_color=c9d1d9&rank_icon=github)](https://github.com/abhay112)
&nbsp;&nbsp;
[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=abhay112&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=6366f1&text_color=c9d1d9&langs_count=8)](https://github.com/abhay112)

</div>
