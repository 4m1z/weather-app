# Infra Repository for weather app

## Overview

This repository contains a very simple app that i have written with golang and react 
to get more familier with graphql. in this project i used gql on backend and apolo client 
on the frontend side which you can find more information regarding them in their respective 
folders(./frontend and ./backend).


## Deployment Instructions

### Prerequisites
- Docker installed on your machine.

### Step-by-Step Deployment

1. **Clone the repo:**

   Clone the following repositories and place them in the same directory structure:

   - **Infra**: [https://github.com/Am1rArsalan/kg-infra](https://github.com/Am1rArsalan/weather-app)

   The directory structure should look like this:

   ```
   frontend/
   backend/
   infra/
   ```

2. **Navigate to the infra folder:**

   ```bash
   cd infra/
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
