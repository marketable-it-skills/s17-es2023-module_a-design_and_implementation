# How to develop and deploy the project?

1. Create a new GitHub repository based on the following template repository: [https://github.com/marketable-it-skills/mits-html-and-vanila-js-v1](https://github.com/marketable-it-skills/mits-html-and-vanila-js-v1)
2. Create your solution in the `/src` folder.
3. When you push a commit to GitHub, an auto-deployment process will start according to the GitHub Actions defined in the repository (`.github` folder). During this process, a Docker image will be built and stored in the Github Container Registry.
4. Modify the following line in the `docker-compose.yml` according to your GitHub username and your repository name: `image: ghcr.io/<your-github-account/<your-repo-name>/<your-repo-name>:latest`
5. Start the Docker container using the `docker compose up -d` command.
6. Your deployment will be accessible at the `http://localhost` URL.
