# Vue.js Application with Docker Deployment
##  Project Overview
This project demonstrates the requirement to set up a **Vue.js** application and successfully deploy it using **Docker**. The primary goal was to create a containerized environment that allows the application to be built and served consistently across different platforms.

---

## Tech Stack
* **Frontend Framework:** Vue 3 (Composition API )
* **Build Tool:** Vite
* **Containerization:** Docker
* **Package Manager:** npm

---

##  Project Structure
The repository follows a clean and minimal structure to support Docker-based deployment:

```text
├── src/                # Main Vue.js source code (components and logic)
├── Dockerfile          # Instructions for building the Docker image
├── vite.config.js      # Vite build tool and dev server configuration
└── package.json        # Project dependencies and scripts used by Docker
```
---
##  Local Installation & Setup
### 1. Clone the Repository 
```bash
git clone https://github.com/rohitkarki483/vue-app
cd vuew-app
```
### 2. Install Dependencies
```bash
npm install
```
### 3.Start Development Server
```bash
npm run dev
```
The application will be available at:
```bash
http://localhost:5173
```

---

 ## Docker Deployment
This project includes a `Dockerfile` to automate the deployment process.

### 1. Build the Image
Run the following command from the vue-app folder:

```bash
docker build -t vue-vite-app .
```
---

### 2. Run the Container
Launch the container and map the internal Vite port (5173) to your local machine:
```bash
docker run -p 5173:5173 vue-vite-app
```
---

### 3. Access the App
open your browser to: http://localhost:5173
