# Landing Page — Dockerized with Nginx + CI/CD

A simple static landing page, containerized with **Docker** and served using **Nginx**, with an automated **CI pipeline** using **GitHub Actions**.

This project is part of a learning path to practice **Docker, Nginx, and CI/CD** together — starting from a basic static site and building up to more advanced deployment pipelines.

---

## 🚀 Tech Stack

- **HTML/CSS** — Static landing page
- **Nginx** — Web server to serve the static site
- **Docker** — Containerization
- **GitHub Actions** — CI pipeline (automated build on every push)

---

## 📂 Project Structure

Landing-Page/
├── index.html # Landing page
├── Dockerfile # Docker build instructions
├── .github/
│ └── workflows/
│ └── docker-build.yml # CI workflow
└── README.md


---

## 🐳 Running Locally with Docker

Build the Docker image:
```bash
docker build -t landing-page .
```

Run the container:
```bash
docker run -d -p 8080:80 landing-page
```

Open in browser:
http://localhost:3000


---

## ⚙️ CI/CD Pipeline

This repo uses **GitHub Actions** to automatically build the Docker image on every push to the `main` branch.

Workflow file: `.github/workflows/docker-build.yml`

Pipeline steps:
1. Checkout the repository code
2. Build the Docker image

You can view the pipeline runs under the **Actions** tab of this repository.

---

## 📌 Learning Goals

This project is built as part of hands-on practice covering:
- Writing a Dockerfile and containerizing a static site
- Serving content through Nginx
- Setting up a basic CI workflow with GitHub Actions
- (Planned next steps) Pushing images to Docker Hub, adding a reverse proxy, load balancing, and SSL

---

## 📄 License

This project is for personal learning purposes.
