# 🌐 **Lab: Architecture Patterns & Design Patterns in Java using GitHub Copilot**

## 🏗️ **Overview**

This lab guides you through implementing **Architecture Patterns** and **Design Patterns** in a **Java Spring Boot application** using **GitHub Copilot**. You will:

* Build a Product Management API
* Implement Clean Architecture
* Use Repository and Factory Patterns
* Use GitHub Copilot for code generation, refactoring, and documentation

---

# 🧩 **1. Understanding Architecture Patterns**

## 🔸 What Are Architecture Patterns?

Architecture patterns define the **overall structure** of applications, focusing on maintainability, scalability, and flow of data.

### Common Architecture Patterns in Java

* Layered Architecture
* Clean Architecture
* Microservices
* Event-Driven Architecture
* Hexagonal Architecture

---

# 🏗️ **2. Understanding Design Patterns**

## 🔸 What Are Design Patterns?

Design patterns solve common design problems at the class and object level.

### Common Java Design Patterns

* **Creational:** Singleton, Factory, Builder
* **Structural:** Adapter, Decorator, Facade
* **Behavioral:** Strategy, Observer, Command

---

# 🧪 **3. Lab Scenario**

You will build a **Spring Boot Product Management API** using:

* Clean Architecture
* Repository Pattern
* Factory Pattern
* GitHub Copilot for development tasks

---

# 🛠️ **4. Project Setup**

## Task 1: Create a Spring Boot Project

Use Spring Initializr or CLI:

```bash
spring init --dependencies=web,data-jpa,h2,validation product-api
cd product-api
```

### ✅ **Copilot Prompt**

```
Create a Clean Architecture folder structure for this Spring Boot project including: domain, application, infrastructure, controllers, services, repositories, dtos.
```

---

# 📦 **5. Implementing Clean Architecture**

## Task 2: Create Domain Model

Create `domain/Product.java`.

### ✅ **Copilot Prompt**

```
Generate a Product entity with id, name, price, and category using javax.validation annotations.
```

---

# 🏛️ **6. Implement Repository Pattern**

## Task 3: Create ProductRepository Interface

File: `domain/repository/ProductRepository.java`

### ✅ **Copilot Prompt**

```
Generate a ProductRepository interface extending JpaRepository with CRUD operations for Product.
```

---

## Task 4: Implement Service Layer

Create `application/service/ProductService.java`.

### ✅ **Copilot Prompt**

```
Generate a ProductService class with methods for create, update, delete, getAll, and getById. Inject ProductRepository using constructor injection.
```

---

# 🏗️ **7. Apply Factory Pattern**

## Task 5: Create ProductFactory

Create `application/factory/ProductFactory.java`.

### ✅ **Copilot Prompt**

```
Create a ProductFactory class with a method createProduct(String name, double price, String category) and return a Product object.
```

---

# 🌐 **8. Build REST Endpoints**

## Task 6: Create ProductController

Create file: `controllers/ProductController.java`.

### Endpoints

* POST /api/products
* GET /api/products
* GET /api/products/{id}
* PUT /api/products/{id}
* DELETE /api/products/{id}

### ✅ **Copilot Prompt**

```
Generate a Spring REST controller named ProductController with CRUD endpoints using ProductService. Return proper ResponseEntity responses and handle exceptions.
```

---

# 🧪 **9. Unit Testing**

## Task 7: Test Factory Pattern

Create: `src/test/java/.../ProductFactoryTest.java`

### ✅ **Copilot Prompt**

```
Write a JUnit test for ProductFactory to verify that createProduct sets the correct fields.
```

---

## Task 8: Test Service Layer

Create: `ProductServiceTest.java`

### ✅ **Copilot Prompt**

```
Write JUnit tests for ProductService using Mockito to mock the ProductRepository.
```

---

# 🤖 **10. Ask Copilot for Architecture Suggestions**

## Task 9: Architecture Review

### ✅ **Copilot Prompt**

```
Analyze this Spring Boot application and suggest improvements based on Clean Architecture, SOLID principles, and Spring best practices.
```

---

# 🚀 **11. Refactor with Copilot**

## Task 10: Improve Code Quality

### Copilot Prompt

```
Refactor ProductController and ProductService to improve code quality, remove duplication, and apply SOLID principles.
```

---

# 📘 **12. BONUS: Auto-generate Documentation**

## Task 11: Create README.md

### Copilot Prompt

```
Generate a professional README.md describing architecture pattern, design patterns used, project structure, build steps, and API endpoints.
```

---

# 🎉 **Lab Completed!**

You have successfully:

* Built a Spring Boot API
* Implemented Clean Architecture
* Applied Repository & Factory Patterns
* Used GitHub Copilot for code, testing, and documentation

You may extend this by adding:

* Architecture diagrams
* Additional patterns (Strategy, Adapter, Singleton)
* Advanced API features or database integration
