# Cloud Microservices Project

## Overview

This project is a cloud-based microservices architecture designed to manage and orchestrate a comprehensive event management system. It leverages modern cloud technologies to provide scalable, resilient, and efficient services for user authentication, event creation, booking, and category management. The system is built using microservices principles, allowing for independent deployment, scaling, and maintenance of individual components.

## Architecture

The project utilizes a microservices architecture deployed on Google Kubernetes Engine (GKE) for container orchestration. Services communicate asynchronously using RabbitMQ as the message broker, ensuring loose coupling and high availability.

### Cloud Architecture

![Cloud Architecture](<diagrams/Cloud%20Architecture%20(Kubernetes%20GKE).png>)

### Messaging Architecture

![Messaging Architecture](<diagrams/Messaging%20Architecture%20(RabbitMQ).png>)

## Services

The system consists of several microservices, each handling specific business domains. The major microservices include:

1. **User Management Service**
   - Handles user registration, login, avatar setting, and password recovery
   - ![User Management State Diagram](diagrams/State%20Diagram%20Login%20%20Register%20%20Set%20Avatar%20%20Forgot%20Password.png)

2. **Event Management Service**
   - Manages event creation and category setup
   - ![Event Creation State Diagram](<diagrams/State%20Diagram(Create%20Category%20&%20Event%20Creation).png>)

3. **Booking Service**
   - Handles event booking processes
   - ![Booking State Diagram](<diagrams/State%20Diagram(Booking%20an%20Event).png>)

Additional supporting microservices may include authentication, notification, payment processing, and logging services, depending on the full implementation.

## Technologies Used

- **Container Orchestration**: Kubernetes (GKE)
- **Messaging**: RabbitMQ
- **Programming Languages**: [Specify if known, e.g., Java, Python, etc.]
- **Databases**: [Specify databases used]
- **Other Tools**: [CI/CD, monitoring, etc.]

## Getting Started

### Prerequisites

- Kubernetes cluster (GKE)
- RabbitMQ instance
- [Other dependencies]

### Installation

1. Clone the repository
2. Deploy to Kubernetes cluster
3. Configure RabbitMQ connections
4. Start the services

### Usage

[Provide basic usage instructions]

## Diagrams

All architectural and state diagrams are available in the `diagrams/` folder:

- Cloud Architecture (Kubernetes GKE)
- Messaging Architecture (RabbitMQ)
- User Management State Diagrams
- Event Management State Diagrams
- Booking State Diagrams

[View Diagrams](./diagrams/)

## Reports

For detailed project reports and documentation, refer to the [Project Report](./Report_Group35.pdf) (if available) or check the diagrams folder for visual documentation.
