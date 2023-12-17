# CMPE 172 Project Journal

## Starbucks Order Flow Simulation
- Utilized Docker and GKE to containerize a microservices-based Starbucks order flow simulation, covering drinks
customization, real-time order tracking, payments across multiple locations, and drink creation
- Enhanced throughput and maintained server health by employing internal and external load balancers through Kong
Ingress, distributed user requests across eight internal API clusters
- Developed 20 REST API endpoints and integrated security measures utilizing Spring Security to safeguard account
and order creation processes
- Integrated RabbitMQ messaging queue to enable asynchronous communication between five microservices,
accelerating real-time updates to coordinate creation and payments of Starbuck orders


## Functionalities - Directories

### Spring-Cashier
Spring Boot application designed to efficiently manage the creation of orders and monitor the status of drinks.

### Starbucks-api
Backend server responsible for handling user requests, including:
- Creation, deletion, activation of Starbucks Cards
- Adding/deducting balance from Starbucks Cards
- Viewing/deleting order status and payments history
- Placing/canceling orders based on location

### Starbucks-app
Mobile application for seamless interactions with Starbucks services. Features include:
- Placing drink orders
- Purchasing drinks
- Viewing and reloading balance on Starbucks Cards
