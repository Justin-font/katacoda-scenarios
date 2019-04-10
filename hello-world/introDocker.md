
# Intro To docker
## What is Docker ?
Docker is a platform for developers and sysadmins to **develop, deploy, and run** applications with containers.
The use of Linux containers to deploy applications is called containerization.
Containers are not new, but their use for easily deploying applications is.

## Why use Docker ?
1. **Reproducibility:** A Docker container is guaranteed to be identical on any system that can run Docker.
2. **Isolation:** Dependencies or settings within a container will not affect any installations or configurations on your computer, or on any other containers that may be running.
3. **Security:** With important caveats (discussed below), separating the different components of a large application into different containers can have security benefits: if one container is compromised the others remain unaffected.
4. **Docker Hub:** For common or simple use cases, such as a LAMP stack, the ability to save images and push them to Docker Hub means that there are already many well-maintained images available.
5. **Environment Management:** Docker makes it easy to maintain different versions of, for example, a website using nginx. You can have a separate container for testing, development, and production on the same Linode and easily deploy to each one.
6. **Continuous Integration:** Docker works well as part of continuous integration pipelines with tools like Travis, Jenkins, and Wercker. Every time your source code is updated, these tools can save the new version as a Docker image, tag it with a version number and push to Docker Hub, then deploy it to production.

## When use Docker ?
1. **Learning new technologies:** To get started with a new tool without spending time on installation and configuration.
2. **App isolation:** If you want to run multiple applications on one server.
3. **Developer teams:** If you have developers working with different setups.

## Security warnning
You must run docker in sudo, but for this tuto we will do it in rootles mode (without sudo)
Warnning on your computer running docker without sudo is highly not recommended for security purpose
Sources: "Why and When to use docker" https://www.linode.com/docs/applications/containers/when-and-why-to-use-docker/

