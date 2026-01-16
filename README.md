# Vue.js Application with Docker Deployment
##  Project Overview
This project fulfills the requirement to set up a modern Vue.js application and successfully deploy it using Docker. The primary goal was to create a containerized environment that allows the application to be built and served consistently across different platforms.

---

## Tech Stack
* **Framework:** Vue 3 (Composition API )
* **Build Tool:** Vite
* **Containerization:** Docker

---

##  Project Structure
The repository is organized as follows to support the containerized workflow:

* **`src/`**: Main Vue.js source code including components and logic.
* **`Dockerfile`**: Contains the instructions for building the Docker image.
* **`vite.config.js`**: Configuration for the Vite build tool and development server.
* **`package.json`**: Defines project dependencies and the scripts used by Docker.
---

 ## Docker Setup
This project includes a `Dockerfile` to automate the deployment process.

### 1. Build the Image
To create the Docker image, run the following command in your terminal:
```bash
docker build -t vue-vite-app .
```
### 2. Run the Container
Launch the container and map the internal Vite port (5173) to your local machine:
```bash
docker run -p 5173:5173 vue-vite-app
```
### 3. Access the App
open your browser to: http://localhost:5173
a
