# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week 2023.

## Diagrama de classes

```mermaid
classDiagram
  class User {
    -name: string
    -account: Account
    -features: Feature[]
    -card: Card
    -news: News[]
  }
  class Account {
    -Number: string
    -Agency: string
    -Balance: float
    -Limit: float
  }
  class Feature {
    -icon: string
    -description: string
  }
  class Card {
    -Number: string
    -Limit: float
  }
  class News {
    -icon: string
    -description: string
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1"  Card
  User "1" *-- "N" News
```
