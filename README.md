# Running the Project with Docker

## Prerequisites

Ensure you have the following installed on your system:
- [Docker](https://www.docker.com/get-started)

## Steps to Run the Application

1. **Navigate to the Project Directory**
   ```sh
   cd path/to/your/project
   ```

2. **Build the Docker Image**
   ```sh
   docker build -t my-frontend-app .
   ```
   - The `-t my-frontend-app` flag names the image as `my-frontend-app`.

3. **Run the Docker Container**
   ```sh
   docker run -p 3000:3000 my-frontend-app
   ```
   - The `-p 3000:3000` flag maps port 3000 of the container to port 3000 of your local machine.

4. **Access the Application**
   Open your browser and go to:
   ```md
   http://localhost:3000
   ```

## Additional Docker Commands

- **Check Running Containers**
  ```sh
  docker ps
  ```

- **Stop the Running Container**
  ```sh
  docker stop <container_id>
  ```

- **Remove All Stopped Containers**
  ```sh
  docker system prune -f
  ```

- **Check Docker Images**
  ```sh
  docker images
  ```

- **Remove a Docker Image**
  ```sh
  docker rmi <image_id>
  ```

- **Rebuild the Docker Image (after changes)**
  ```sh
  docker build --no-cache -t my-frontend-app .
  ```

- **Run the Container in Detached Mode**
  ```sh
  docker run -d -p 3000:3000 my-frontend-app
  ```

- **Check Docker Logs**
  ```sh
  docker logs <container_id>
  ```

## Notes
- Ensure port `3000` is not in use by other applications.
- Modify the `Dockerfile` or use `.env` if you need custom environment variables.

## Frontend Libraries to be used
- [Motion Primitives](https://motion-primitives.com/)
- [Animata Design](https://animata.design/)
- [Lukacho](https://ui.lukacho.com/)
- [Mantine UI](https://ui.mantine.dev/)
- [Aceternity UI](https://ui.aceternity.com/) - recommended
- [Daisy UI](https://daisyui.com/)
- [Shadcn UI](https://ui.shadcn.com/) - recommended
- [Hero UI](https://www.heroui.com/)


