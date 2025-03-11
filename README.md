#Bootcamp Avanade 2025
Java RESTful API criada para o Bootcamp Avanade 2025.

## Diagrama de classes

...mermaid
classDiagram
    class Client {
        +String name
        +Account account
        +Feature[] features
        +OrderForSweets orderForSweets
        +News[] news
    }

    class Account {
        +String client
        +String credit
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
