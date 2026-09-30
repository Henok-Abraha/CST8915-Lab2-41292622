# CST8915 Lab 2: Algonquin Pet Store on Azure VM

**Student Name:** Henok Abraha  
**Student ID:** 41292622  
**Course:** CST8915 Full-stack Cloud-native Development  
**Semester:** Fall 2026  

---

## Demo Video

[Watch Demo Video](https://www.youtube.com/watch?v=E-7F2XykC04)

---
## inks to the  service repositories

[Store Front](https://github.com/Henok-Abraha/store-front)
[Product Service](https://github.com/Henok-Abraha/product-service)
[Order Service](https://github.com/Henok-Abraha/order-service)



### What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?

I changed the orderservice and product-service to use environment variables instead of putting the configurations directly inside the code. The product service gets the port 3000 from the .env file and the order service gets the port and RabbitMQ connection from the .env file. I also used RabbitMQ as a separate backing service running on its own Azure VM.

### Why is it important to use environment variables instead of hard-coding configurations in your application

Using environment variables is important because we don't have to change the code every time a configuration changes. It also helps us hide important information like passwords and connection strings, so they don't get uploaded to GitHub.

### Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?

Having separate repositories for each microservice is important because each service can work independently. We can update or fix one service without changing the other services. It also makes it easier to deploy and scale each service separately.

---


