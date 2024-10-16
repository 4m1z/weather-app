# Infra Repository for weather app

## Overview

The **infra** repository manages the deployment process for the full-stack weather application (frontend and backend) using Docker Compose. This setup enables seamless orchestration of the frontend, backend, and external services.

## Project Structure

```
infra/
    └── docker-compose.yml
    └── README.md
```

## Deployment Instructions

### Prerequisites
- Docker installed on your machine.

### Step-by-Step Deployment

1. **Clone the repositories:**

   Clone the following repositories and place them in the same directory structure:

   - **Frontend (fe)**: [https://github.com/Am1rArsalan/fe-kg](https://github.com/Am1rArsalan/fe-kg)
   - **Backend (be)**: [https://github.com/Am1rArsalan/be-kg](https://github.com/Am1rArsalan/be-kg)
   - **Infra**: [https://github.com/Am1rArsalan/kg-infra](https://github.com/Am1rArsalan/kg-infra)

   The directory structure should look like this:

   ```
   fe-kg/
   be-kg/
   kg-infra/
   ```

2. **Navigate to the infra folder:**

   ```bash
   cd kg-infra/
   ```

3. **Build and run the services:**

   Run the following command to build and start all services in detached mode:

   ```bash
   docker compose up --build -d
   ```

4. **Check the status of the containers:**

   You can check the logs of the frontend and backend containers by running:

   ```bash
   docker compose logs frontend
   docker compose logs backend
   ```

5. **Access the application:**

   Once everything is up and running, you can access the full-stack application on [http://localhost:3000](http://localhost:3000).
