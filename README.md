# AVANADE Boot Camp 2025
Java RESTful API criada para o Boot Camp 2025 na plataforma da DIO em parceria com a AVANADE.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +Card card
        +List~Feature~ features
        +List~News~ news
    }
    
    class Account {
        +String number
        +String agency
        +double balance
        +double limit
    }
    
    class Card {
        +String number
        +double limit
    }
    
    class Feature {
        +String icon
        +String description
    }
    
    class News {
        +String icon
        +String description
    }
    
    User *-- Account
    User *-- Card
    User *-- "*" Feature
    User *-- "*" News
```
