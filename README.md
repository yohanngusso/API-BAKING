# Santander Dev Week 2023
Java RESTful API criada para o Santander Dev Week

## Diagrama de Classes


```mermaid
classDiagram
    class User {
        +String name
    }
    
    class Account {
        +String agencia
        +String number
        +Number balance
        +Number limit
    }
    
    class Feature {
        +String icon
        +String description
    }
    
    class Card {
        +String number
        +Number limit
    }
    
    class News {
        +String icon
        +String description
    }

    User "1" *-- "1" Account : possui
    User "1" *-- "N" Card : possui
    User "1" *-- "N" Feature : tem
    User "1" *-- "N" News : recebe
  ```


