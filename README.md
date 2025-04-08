# Santander Dev Week 2025

Este projeto foi desenvolvido como parte do bootcamp **DIO + Avanade**, com foco na construção de uma API RESTful utilizando **Java** e **Spring Boot**.

## 💼 Objetivo
Simular um ambiente bancário digital, exibindo informações de usuário, conta, cartão, recursos disponíveis e notificações — seguindo boas práticas de arquitetura e organização de código.

## 🔧 Tecnologias utilizadas
- **Java 17**
- **Spring Boot**
- **Gradle**
- **VS Code**
- **Git & GitHub**

## 🚀 Funcionalidades implementadas
- Consulta de dados bancários do usuário
- Informações da conta e cartão de crédito
- Lista de funcionalidades disponíveis
- Simulação de notificações bancárias e novidades

## Diagrama de classes 

```mermaid

classDiagram
  class User {
    +String name
    +Account account
    +Feature[] features
    +Card card
    +News[] news
    +Notification[] notifications
  }

  class Account {
    +String number
    +String agency
    +float balance
    +float limit
  }

  class Feature {
    +String icon
    +String description
  }

  class Card {
    +String number
    +float limit
  }

  class News {
    +String icon
    +String description
  }

  class Notification {
    +String message
    +String date
    +bool read
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News
  User "1" *-- "N" Notification
```

## 👩‍💻 Autora
**Raíssa Monteiro**  
Desenvolvedora em formação, apaixonada por tecnologia, back-end e criação de soluções que gerem impacto.  
📧 raissasbmonteiro@gmail.com 
🌐 [LinkedIn](https://www.linkedin.com/in/ra%C3%ADssa-monteiro-90b156226/) 

