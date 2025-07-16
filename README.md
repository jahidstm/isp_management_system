# 🌐 ISP Management System  
**Object-Oriented Design Course Project (Java)**  
*A scalable system for managing Internet Service Provider operations*  

![Java](https://img.shields.io/badge/Java-11%2B-orange)
![OOP](https://img.shields.io/badge/Design-Object_Oriented-brightgreen)
![Status](https://img.shields.io/badge/Status-Active-success)

---

## 🚀 Project Overview  
This Java-based ISP Management System demonstrates **core OOP principles** including:  
✔ Encapsulation (Private fields + Getters/Setters)  
✔ Inheritance (Abstract classes)  
✔ Polymorphism (Method overriding)  
✔ SOLID Design Patterns  

Designed for:  
- Customer account management  
- Bandwidth allocation tracking  
- Automated billing  

---

## ✨ Key Features  
- **Customer Module**:  
  - Plan subscription  
  - Usage tracking  
- **Admin Module**:  
  - User CRUD operations  
  - Revenue reports  
- **Technical Core**:  
  - Rate-limiting system  
  - Invoice generation  

---

## 🏗 Class Diagram  
```mermaid
classDiagram
    class Customer{
        -String name
        -String email
        +subscribePlan()
        +makePayment()
    }
    class Admin{
        +addCustomer()
        +generateReport()
    }
    class BillingSystem{
        +calculateUsage()
        +generateInvoice()
    }
    Customer --|> BillingSystem
    Admin ..> Customer
