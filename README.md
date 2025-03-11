#Bootcamp Avanade 2025
Java RESTful API criada para o Bootcamp Avanade 2025.

## Diagrama de classes

...mermaid
classDiagram
    class Matricula {
        +String name
        +Account account
        +Feature[] features
        +OrderForSweets orderForSweets
        +News[] news
    }

    class Account {
        +String matricula
        +String bonus
        +String debt
    }

    class Feature {
        +String icon
        +String description
    }

    class OrderForSweets {
        +String cake
    }

    class News {
        +String icon
        +String description
    }

    Client --> Account
    Client --> Feature : has
    Client --> OrderForSweets : has
    Client --> News : has
...
