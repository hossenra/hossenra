<h1 align="center">Hi, I'm Razibul Hossen 👋</h1>
<h3 align="center">Full-Stack Developer · Cloud & DevOps Engineer · Berlin, Germany</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Currently-Full--Stack%20Developer%20@%20Hitachi%20Rail-blue?style=flat-square" alt="Currently Full-Stack Developer at Hitachi Rail" />
  <img src="https://img.shields.io/badge/Completed-DevOps%20%26%20Cloud%20Bootcamp-success?style=flat-square" alt="Completed DevOps and Cloud Engineering Bootcamp" />
  <img src="https://img.shields.io/badge/Preparing-AWS%20SAA--C03-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="Preparing for AWS Solutions Architect Associate" />
  <img src="https://img.shields.io/badge/Open%20to-DevOps%20%7C%20Cloud%20%7C%20Full--Stack%20roles-black?style=flat-square" alt="Open to DevOps, Cloud and Full-Stack roles" />
</p>

I've spent three years building web applications with **React, TypeScript, Node.js and SQL** for German companies. Now I'm focused on the other half of the job: **getting code deployed safely and keeping it running**. That means CI/CD pipelines, Docker, AWS, Linux and Nginx, with Kubernetes and Terraform next.

Currently a **Full-Stack Developer (Werkstudent) at Hitachi Rail** in Stuttgart, alongside an M.Sc. in Physics at BTU Cottbus-Senftenberg. I recently completed bongoDev's **DevOps & Cloud Engineering Bootcamp**.

---

### ⚡ What I'm working on now

- 🎓 **DevOps & Cloud Engineering Bootcamp (bongoDev)**, completed Oct 2026 with certificate: Linux, networking, Python, Docker, Kubernetes, Terraform, Ansible, AWS, GitHub Actions, Prometheus and Grafana
- 🤖 **Mastering Agentic Coding** ([LWHH](https://lwhh.org/courses/mastering-agentic-coding)), nearly done: working with AI coding agents, Git workflows with agents, custom skills, sandboxing, and reviewing agent-written code
- 🧩 **System Design** ([systemflow.dev](https://systemflow.dev/)): scalability, caching, databases, messaging and distributed systems
- ☁️ Preparing for **AWS Solutions Architect – Associate (SAA-C03)**
- 📦 Moving **ZapShift** to **AWS ECS/ECR** with Terraform and Prometheus/Grafana monitoring
- 🇩🇪 Improving my German from B1 toward B2

---

### 🚀 Featured projects

#### 📦 ZapShift, a parcel delivery platform · [client](https://github.com/hossenra/Zap-shift-client) · [server](https://github.com/hossenra/Zap-shift-server)

A full-stack delivery platform with dashboards for customers, riders and admins, shipment tracking with a status timeline, a coverage map and server-verified Stripe payments.

- **CI/CD with GitHub Actions** on both repos: lint, build and tests on every push and pull request
- **API pipeline:** tests on a Node 20 and 22 matrix → Docker build → container smoke test against `/health` → deploy to Render → health check against production
- **Frontend pipeline:** lint and build → build artifact → deploy to Vercel, only from `main`
- **Docker image:** `node:22-alpine`, production dependencies only, runs as the non-root `node` user, built-in `HEALTHCHECK`

`React 19` `TanStack Query` `React Router 7` `Leaflet` `Node.js` `Express 5` `MongoDB` `Firebase Auth` `Stripe` `Docker` `GitHub Actions`

#### 🌐 Zero-downtime deployment for my portfolio website

A static site served by **Nginx on Ubuntu EC2** and deployed by **GitHub Actions**:

- Validates the HTML and checks for broken local links before anything ships
- Connects with a **short-lived SSH key via EC2 Instance Connect**, so no private key is stored in GitHub. The IAM policy is limited to one instance and one user.
- Unpacks each release into `releases/<commit>` and goes live with a single **symlink switch**
- Runs `nginx -t`, reloads, then **health-checks** `/health` and `/` both on the server and over the internet
- **Rolls back automatically** to the previous release if any check fails, and keeps the last five releases

`AWS EC2` `IAM` `EC2 Instance Connect` `Nginx` `GitHub Actions` `Bash` `Python`

#### ☸️ [k8s-deep-dive](https://github.com/hossenra/k8s-deep-dive)

My hands-on Kubernetes lab on a local **kind** cluster, with manifests for Pods, ReplicaSets, Deployments, DaemonSets, Services, Ingress, Namespaces and PersistentVolumes/Claims, plus the Kubernetes Dashboard setup.

`Kubernetes` `kind` `kubectl` `YAML` `Docker`

---

### 💼 Things I've shipped at work

- **Cut average dashboard load times by about 30%** by optimising the SQL queries behind reporting dashboards *(Hitachi Rail)*
- **Built 10+ accessible, reusable React and MUI components** across four product areas *(Hitachi Rail)*
- **Reduced reported UI bugs by about 25%** while building and improving 5+ user-facing React features *(PVision)*
- **Raised test coverage by about 40%** with Jest unit and integration tests and regular code reviews *(Q4U Experience Design Studio)*
- **Developed 15+ REST endpoints** with Node.js and Express on MongoDB, and on PostgreSQL via Prisma *(Q4U)*
- **Supported Docker-based local development** across the team, reducing environment drift *(Q4U)*

---

### 🛠️ Tech stack

| Area | Technologies |
|---|---|
| **Frontend** | ![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=white&style=flat-square) ![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white&style=flat-square) ![Next.js](https://img.shields.io/badge/-Next.js-000000?logo=nextdotjs&logoColor=white&style=flat-square) ![Redux](https://img.shields.io/badge/-Redux-764ABC?logo=redux&logoColor=white&style=flat-square) ![Tailwind](https://img.shields.io/badge/-Tailwind-06B6D4?logo=tailwindcss&logoColor=white&style=flat-square) |
| **Backend & data** | ![Node.js](https://img.shields.io/badge/-Node.js-339933?logo=nodedotjs&logoColor=white&style=flat-square) ![Express](https://img.shields.io/badge/-Express-000000?logo=express&logoColor=white&style=flat-square) ![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?logo=postgresql&logoColor=white&style=flat-square) ![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white&style=flat-square) ![Prisma](https://img.shields.io/badge/-Prisma-2D3748?logo=prisma&logoColor=white&style=flat-square) |
| **CI/CD & delivery** *(used in my projects)* | ![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white&style=flat-square) ![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white&style=flat-square) ![AWS EC2](https://img.shields.io/badge/-AWS%20EC2-232F3E?logo=amazonaws&logoColor=white&style=flat-square) ![Nginx](https://img.shields.io/badge/-Nginx-009639?logo=nginx&logoColor=white&style=flat-square) ![Linux](https://img.shields.io/badge/-Linux-FCC624?logo=linux&logoColor=black&style=flat-square) ![Bash](https://img.shields.io/badge/-Bash-4EAA25?logo=gnubash&logoColor=white&style=flat-square) ![Jest](https://img.shields.io/badge/-Jest-C21325?logo=jest&logoColor=white&style=flat-square) |
| **Cloud & DevOps** *(trained in, building depth)* | ![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?logo=kubernetes&logoColor=white&style=flat-square) ![Terraform](https://img.shields.io/badge/-Terraform-7B42BC?logo=terraform&logoColor=white&style=flat-square) ![Ansible](https://img.shields.io/badge/-Ansible-EE0000?logo=ansible&logoColor=white&style=flat-square) ![Prometheus](https://img.shields.io/badge/-Prometheus-E6522C?logo=prometheus&logoColor=white&style=flat-square) ![Grafana](https://img.shields.io/badge/-Grafana-F46800?logo=grafana&logoColor=white&style=flat-square) ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=flat-square) ![Jenkins](https://img.shields.io/badge/-Jenkins-D24939?logo=jenkins&logoColor=white&style=flat-square) |
| **AI-assisted development** | Agentic coding workflows, Kilo Code, Command Code, reviewing agent-written code |

---

### 🎓 Education

- **M.Sc. Physics**, BTU Cottbus-Senftenberg *(Oct 2023 – present)*
- **B.Sc. Physics**, National University of Bangladesh *(2010 – 2014)*

Languages: Bengali (native), English (C1), German (B1, working toward B2). Valid German residence and work permit.

---

### 📊 GitHub stats

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=hossenra&show_icons=true&hide_border=true" height="165" alt="GitHub stats" />
  <img src="https://streak-stats.demolab.com/?user=hossenra&hide_border=true" height="165" alt="GitHub streak" />
</p>

---

### 🌐 Let's connect

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/razibul-hossen-b0573aa3/)
[![Email](https://img.shields.io/badge/-smraju1234@gmail.com-D14836?logo=gmail&logoColor=white&style=flat-square)](mailto:smraju1234@gmail.com)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white&style=flat-square)](https://github.com/hossenra)
