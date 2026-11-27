## Hosting Plan

We want to utilize a hosted service to deploy Gist & Grind to the web so that it will be accessible online. By this, we will simplify the process of deployment and decrease our workload of maintaining a server.

### Deployment Process

1. First, we are going to push our application code to our GitHub repository.
2. Our hosting will connect to our GitHub repository and build our application.
3. We will set up a PostgreSQL database, connect it to the backend, and use `DATABASE_URL` variable.
4. We will configure the necessary environment variables and secrets using the hosted service.
5. After deployment, our hosting will give us a live HTTPS link, which students will be able to access.

### Reasons Behind Our Decision to Go with a Managed Hosting Service

- It simplifies the process of deploying updates.
- It simplifies maintaining servers manually.
- It ensures using HTTPS for securing connections.
- Allows concentrating efforts on development of core functionality.

### Further Improvements

As Gist & Grind grows, we may need to upgrade our hosting plan or move to a different provider if the number of users increases, the cost becomes too high, or we need more control over the server.

We will also consider choosing a hosting region close to our users to improve performance.
