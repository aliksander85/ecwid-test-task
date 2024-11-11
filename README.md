# ECWID Test Task

This project includes two Vue applications: `widget-recent` and `settings`, both running through Docker Compose.

## Requirements

Docker and Docker Compose should be installed on your machine.

## Getting Started

1. Clone the repository:
```bash
git clone <repository-link>
cd ecwid-test-task
```

2. Run the project:
```bash
docker-compose up --build
```

3.	Access the applications:
•	**widget-recent**: http://localhost:8081
•	**settings**: http://localhost:8082

## Docker Compose Configuration

The docker-compose.yml file defines two services:
•	**widget-recent**: Mapped to port 8081 on your local machine.
•	**settings**: Mapped to port 8082 on your local machine.

Each application has its own Dockerfile to handle dependencies and build processes. Both applications run in the same Docker network, vue-network, for isolated communication.

## Notes

This project is designed to be easily understandable and portable. You can build and launch the entire project using a single entry point (docker-compose up --build), making it convenient for deployment on any machine.