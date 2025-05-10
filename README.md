# Microservices-Task

## Overview
This document provides details on testing various services after running the `docker-compose` file. These services include User, Product, Order, and Gateway Services. Each service has its own endpoints for testing purposes.

---
## Instructions
1. Start all services using the `docker-compose` file:
   ```
   docker-compose up
   ```
2. Once the services are running, use the above endpoints to verify the functionality.


## Services and Endpoints

### **Gateway Service**
- **Base URL:** `http://localhost:3003`
- **Endpoints:**
  - **Health:**  
    ```
    curl http://localhost:3003/health
    ```
    
![image](https://github.com/user-attachments/assets/6a2e14ae-2cb7-4cd3-b671-b6c0da6cc3f0)

  - **Users:**  
    ```
    curl http://localhost:3003/api/users
    ```
    
![image](https://github.com/user-attachments/assets/853e3eb9-22eb-4170-a02c-9314c8ffd41a)

  - **Products:**  
    ```
    curl http://localhost:3003/api/products
    ```
    
![image](https://github.com/user-attachments/assets/6daef490-2b8d-465a-a24b-b8dab4a1b0fb)

  - **Orders:**  
    ```
    curl http://localhost:3003/api/orders
    ```
    
![image](https://github.com/user-attachments/assets/665b3d0d-d857-49a1-90c0-4c04b0aa920d)

---

### **Order Service**
- **Base URL:** `http://localhost:3002`
- **Endpoints:**
   - **Health:**  
    ```
    curl http://localhost:3002/users
    ```
    
![image](https://github.com/user-attachments/assets/134f0c91-59e4-4603-bfa7-4c0fb431d430)

  - **List Orders:**  
    ```
    curl http://localhost:3002/orders
    ```
    
![image](https://github.com/user-attachments/assets/ad21c902-a583-44e7-ba43-c3ba20bfb1ec)

---

### **Product Service**
- **Base URL:** `http://localhost:3001/api`
- **Endpoints:**
  - **Health:**  
    ```
    curl http://localhost:3001/users
    ```
    
![image](https://github.com/user-attachments/assets/3bda4540-37a8-4a5d-85b7-88991323f6f5)

  - **Products:**  
    ```
    curl http://localhost:3001/products
    ```
    
![image](https://github.com/user-attachments/assets/812d0c62-7fa1-4603-a0f7-1a2aa1a8c347)

---

### **User Service**
- **Endpoints:**
  - **Health:**
    ```
    curl http://localhost:3000/Health
    ```
    
![image](https://github.com/user-attachments/assets/582757b8-3842-4b81-92ac-b946a75e5bbf)

  - **Users:**
    ```
    curl http://localhost:3000/users
    ```
    
![image](https://github.com/user-attachments/assets/4b9f82a3-a76f-4099-b24a-25effdd0324f)

---

Happy testing!
