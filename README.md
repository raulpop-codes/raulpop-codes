<p align="center">
  <img src="assets/banner.svg" alt="Raul Pop — Automation &amp; Applied Informatics @ TUCN" width="100%">
</p>

## Hi, I'm Raul 👋

<img src="assets/hero.svg" align="right" width="400" alt="">

**Automation & Applied Informatics student @ TUCN**

I like the part of engineering where control theory meets actual software — writing the math myself, then wrapping it in something you can click. Most of what I build ends up being desktop tools, backends and databases that have to hold up under real use, not just compile.

I'm in my third year of **Automation and Applied Informatics** at the *Faculty of Automation and Computer Science*, **Technical University of Cluj-Napoca** — 9.78/10 over the first two years, on the Academic Performance Scholarship. In parallel I'm going through the **Teacher Training Program** at the Psychopedagogical Specialty Department (DSPP).

My projects tend to sit on both sides of that line: a C++ tool that does root locus, Bode and Runge–Kutta simulation with a math library written from scratch; a Java inventory manager with Redis-backed sessions and rate limiting; a 17-table MySQL schema with business rules enforced at schema level; and a live .NET workout app deployed on Oracle Cloud behind Caddy and Cloudflare.

Lately I've been working on **system identification in MATLAB/Simulink** — fitting a second-order model to an active suspension from its damped response, then validating state-space and transfer-function forms against measured data.

Outside work: sci-fi and fantasy, guitar, the gym and cooking.

<br clear="right">

---

## 🛠️ Tech Stack

**Languages**

![C#](https://img.shields.io/badge/C%23-0E2A1F?style=for-the-badge&logo=csharp&logoColor=3FB27F)
![Java](https://img.shields.io/badge/Java-0E2A1F?style=for-the-badge&logo=openjdk&logoColor=3FB27F)
![C](https://img.shields.io/badge/C-0E2A1F?style=for-the-badge&logo=c&logoColor=3FB27F)
![C++](https://img.shields.io/badge/C++-0E2A1F?style=for-the-badge&logo=cplusplus&logoColor=3FB27F)
![SQL](https://img.shields.io/badge/SQL-0E2A1F?style=for-the-badge&logo=mysql&logoColor=3FB27F)
![MATLAB](https://img.shields.io/badge/MATLAB-0E2A1F?style=for-the-badge&logo=mathworks&logoColor=3FB27F)

**Frameworks & Libraries**

![.NET](https://img.shields.io/badge/.NET-0E2A1F?style=for-the-badge&logo=dotnet&logoColor=3FB27F)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-0E2A1F?style=for-the-badge&logo=dotnet&logoColor=3FB27F)
![EF Core](https://img.shields.io/badge/EF%20Core-0E2A1F?style=for-the-badge&logo=nuget&logoColor=3FB27F)
![React](https://img.shields.io/badge/React-0E2A1F?style=for-the-badge&logo=react&logoColor=3FB27F)
![Swing](https://img.shields.io/badge/Swing-0E2A1F?style=for-the-badge&logo=openjdk&logoColor=3FB27F)
![SFML](https://img.shields.io/badge/SFML-0E2A1F?style=for-the-badge&logo=sfml&logoColor=3FB27F)

**Databases**

![MySQL](https://img.shields.io/badge/MySQL-0E2A1F?style=for-the-badge&logo=mysql&logoColor=3FB27F)
![Redis](https://img.shields.io/badge/Redis-0E2A1F?style=for-the-badge&logo=redis&logoColor=3FB27F)

**Tools & Platforms**

![Git](https://img.shields.io/badge/Git-0E2A1F?style=for-the-badge&logo=git&logoColor=3FB27F)
![Docker](https://img.shields.io/badge/Docker-0E2A1F?style=for-the-badge&logo=docker&logoColor=3FB27F)
![Caddy](https://img.shields.io/badge/Caddy-0E2A1F?style=for-the-badge&logo=caddy&logoColor=3FB27F)
![Cloudflare](https://img.shields.io/badge/Cloudflare-0E2A1F?style=for-the-badge&logo=cloudflare&logoColor=3FB27F)
![Oracle Cloud](https://img.shields.io/badge/Oracle%20Cloud-0E2A1F?style=for-the-badge&logo=oracle&logoColor=3FB27F)
![Simulink](https://img.shields.io/badge/Simulink-0E2A1F?style=for-the-badge&logo=mathworks&logoColor=3FB27F)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-0E2A1F?style=for-the-badge&logo=githubactions&logoColor=3FB27F)

---

## 🚀 Projects

### [NoMoreQuiting](https://github.com/raulpop-codes/NoMoreQuiting) · [nomorequiting.com](https://nomorequiting.com)

Live workout-tracking web app, built in a two-person team — Gym and Fitness sections, custom categories, live session logging (sets/reps/weight) and friend leaderboards. I work on the ASP.NET Core backend and the MySQL schema behind a 40+ exercise catalog, plus deployment: Docker Compose on Oracle Cloud, served through Caddy with automatic HTTPS and Cloudflare.

`C#` · `ASP.NET Core` · `React` · `MySQL` · `Redis` · `Docker`

### [Control Systems Visualization Tool](https://github.com/raulpop-codes/Control-Systems-Visualization-Tool) [![CI](https://img.shields.io/github/actions/workflow/status/raulpop-codes/Control-Systems-Visualization-Tool/ci.yml?style=flat-square&label=CI&labelColor=0E2A1F&color=0E2A1F)](https://github.com/raulpop-codes/Control-Systems-Visualization-Tool/actions/workflows/ci.yml)

Desktop tool for analyzing linear control systems: state-space ↔ transfer-function conversion (Faddeev–LeVerrier, controllable canonical form), an interactive root locus with branch tracking and a live gain slider, step and impulse response via fourth-order Runge–Kutta, plus Bode, Nichols and Nyquist views with gain and phase margins. The complex-number, matrix and polynomial layer (Durand–Kerner root-finding) is written from scratch, with no external math dependencies.

`C++17` · `SFML 3` · `Make`

### [Smart Inventory System](https://github.com/raulpop-codes/Smart-Inventory-System) [![CI](https://img.shields.io/github/actions/workflow/status/raulpop-codes/Smart-Inventory-System/ci.yml?style=flat-square&label=CI&labelColor=0E2A1F&color=0E2A1F)](https://github.com/raulpop-codes/Smart-Inventory-System/actions/workflows/ci.yml)

Desktop inventory and crafting manager tracking 600+ resources and items, aggregating requirements across pending blueprints and reporting exactly what's still missing. Layered architecture with the Repository pattern (MySQL and Redis behind the same interfaces) and Observer-driven readiness alarms; auth uses bcrypt hashing, Redis-backed sessions, rate limiting and device lockout.

`Java 21` · `Swing` · `MySQL` · `Redis` · `Docker`

### [Microcontroller Distributor Database](https://github.com/raulpop-codes/MicrocontrollerFirmDatabase) [![CI](https://img.shields.io/github/actions/workflow/status/raulpop-codes/MicrocontrollerFirmDatabase/ci.yml?style=flat-square&label=CI&labelColor=0E2A1F&color=0E2A1F)](https://github.com/raulpop-codes/MicrocontrollerFirmDatabase/actions/workflows/ci.yml)

A 17-table relational schema normalized to 3NF, modeling a distributor's catalog, suppliers, quality testing and sales pipeline, with three many-to-many relationships resolved through junction tables. Business rules are enforced at schema level — PK/FK, UNIQUE, CHECK with REGEXP validation, a BEFORE INSERT trigger and four analytical reporting views.

`MySQL`

### [Active Suspension System Identification](https://github.com/raulpop-codes/active-suspension-system-identification) <sub>· in progress</sub>

System identification on an active suspension: a second-order model fitted by linear regression on the damped response envelope, then state-space and transfer-function representations validated against filtered measured data. Built to grow with more identification methods over time.

`MATLAB` · `Simulink`

---

## 🎮 And one just for fun

**[Bob Năstrușnicul](https://github.com/raulpop-codes/BobNastrusnicul)** — a 2D top-down maze game in Unity, my first project in both Unity and C#. Every piece of art (character, environment, UI, all 9 collectible items) is hand-drawn by me in Inkscape, and it has a full working inventory system. Originally a high-school certification project; a playable Windows build is in Releases.

`Unity` · `C#` · `Inkscape`

---

<p align="center">
  <a href="https://linkedin.com/in/raulpop-dev"><img src="https://img.shields.io/badge/LinkedIn-0E2A1F?style=for-the-badge&logo=linkedin&logoColor=3FB27F"></a>
  <a href="mailto:2005.raul.pop.2005@gmail.com"><img src="https://img.shields.io/badge/Email-0E2A1F?style=for-the-badge&logo=gmail&logoColor=3FB27F"></a>
</p>

<p align="center"><sub>Romanian (native) · English (C1) · German (A2)</sub></p>
