# Hi, I'm Oleg 👋 
### Senior Full-Stack & Mobile Engineer

[🇬🇧 English] | [🇷🇺 Посмотреть на русском](README.ru.md)

I am a software engineer with 7+ years of commercial experience specializing in end-to-end application architecture, high-performance mobile runtimes, resilient backend systems, and web security.

---

## 🛠️ Tech Stack & Expertise

* **Backend:** Node.js (TypeScript) • PHP (Laravel, Filament) • REST API • GraphQL
* **Mobile & Frontend:** TypeScript • React Native • @shopify/react-native-skia • Reanimated v4 • React • Next.js
* **Databases & Infra:** PostgreSQL • MySQL • ClickHouse • Redis • Docker • Firebase

---

## 🏗️ Production-Grade Showcases

*Below are isolated production-grade modules designed to showcase how I solve complex architectural, rendering, and security bottlenecks. My commercial code is safely protected under NDAs.*

### 1. 📊 [High-Performance Interactive Canvas / Timeline](https://github.com/OlegAlb/Timeline)
**Stack:** *React Native, React Native Skia, Reanimated v3, Feature-Sliced Design (FSD)*
A repository showcasing how to bypass the **React re-render bottleneck ($O(N)$ overhead)** when dealing with complex, fast-changing interactive components (like booking grids, timelines, or financial charts) on lower-end mobile devices.
* **GPU-Accelerated Rendering:** Eliminates heavy React view hierarchies by rendering the entire interactive timeline layout node graph on a single Skia Canvas.
* **Zero Main-Thread Blocking:** Offloads real-time gesture interactions (Hit-Testing for Drag-and-Drop, resizing, and splitting dynamic blocks) entirely to the UI thread using **Reanimated Worklets**.
* **Dynamic Graphs via Bezier Paths:** Features "rubbery" connection lines between active cards calculated dynamically via Cubic Bezier Curves (`Skia.Path.Make() / cubicTo`) rendering smoothly at stable 60/120 FPS during active interaction.

### 2. 🛡️ [Zero-Trust Upload Pipeline & Async Logging Engine](https://github.com/OlegAlb/SecureUploadService)
**Stack:** *Node.js / TypeScript, Redis (Queues), ClickHouse, Docker*
A backend microservice implementing strict defense-in-depth strategies against **OWASP Top 10 vulnerabilities (specifically Arbitrary File Upload & RCE)** combined with a high-throughput async logging pipeline.
* **RCE & Injection Mitigation:** Implements streaming file validation checking file signatures (Magic Bytes) on the fly, enforces filename obfuscation, and applies absolute file-system privilege isolation.
* **Asynchronous Execution Container:** Offloads resource-heavy security scanning and processing pipelines out of the request-response cycle using **Redis-backed worker queues** for instant client responses.
* **High-Throughput Audit Engine:** Implements bulk-insertion patterns of network/security logs into column-oriented **ClickHouse** storage to prevent I/O disk throttling under heavy load or brute-force tracking.

---

## 📫 How to reach me:

* **Telegram:** [@G1glz](https://t.me/G1glz)
* **LinkedIn:** [Oleg Albaut](https://www.linkedin.com/in/oleg-albaut-638a86272/)
* **Email:** [oleg.albaut@outlook.com](mailto:oleg.albaut@outlook.com)
