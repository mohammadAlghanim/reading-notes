# What are the key components of a Docker container, and how do they help streamline the development and deployment of applications?
The key components of a Docker container are as follows:

Docker Image: It is a lightweight, standalone, and executable software package that includes everything needed to run an application, including the code, runtime, system tools, system libraries, and dependencies. Docker images are built based on a set of instructions called Dockerfile, which specifies the configuration and setup of the application environment.

Docker Container: A container is an instance of a Docker image that can be run, deployed, and managed independently. It encapsulates the application and its dependencies in an isolated environment, providing process-level isolation and resource constraints. Containers are portable, consistent, and reproducible, enabling easy deployment across different environments.

Docker Engine: It is the runtime environment that manages the containers. Docker Engine provides the necessary tools and libraries to build, run, and manage Docker containers. It consists of the Docker daemon, which runs in the background, and the Docker client, which provides a command-line interface (CLI) for interacting with the daemon.

Docker Registry: A registry is a centralized repository that stores Docker images. The default registry is Docker Hub, which is a public registry hosting a vast number of pre-built images. However, private registries can also be used to store and distribute custom Docker images within an organization.
# Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates.
Building a library website using Django typically involves the following primary steps, including the essential components like models, views, and templates:

Set up Django Project:

Install Django using pip or any package manager.
Create a new Django project using the django-admin startproject command.
Navigate to the project directory.
# Can you explain the primary differences between Django and Django REST framework?
Django and Django REST framework (DRF) are both frameworks for web development in Python, but they serve different purposes and have distinct features. Here are the primary differences between Django and Django REST framework:

Core Functionality:

Django: Django is a high-level web framework primarily focused on building full-stack web applications. It provides a robust set of features for database modeling, URL routing, HTML templating, form handling, user authentication, session management, and more. Django is well-suited for building traditional server-rendered web applications.
Django REST framework: DRF is an extension of Django that specifically focuses on building Web APIs (Application Programming Interfaces). It provides additional features and tools to facilitate the development of RESTful APIs. DRF adds a layer on top of Django, allowing you to build APIs with powerful serialization, request/response handling, authentication, permission management, and other RESTful functionalities.