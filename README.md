# spring_railway
A simple project with railway integration


# Class diagram 

``` mermaid
classDiagram
    class User {
      +String name
    }
    
    class Account {
      +String number
      +String agency
      +Float balance
      +Float limit
    }

    class Feature {
      +String icon
      +String description
      +String path
    }
    
    class Card {
      +String number
      +Float limit
    }
    
    class News {
      +String icon
      +String description
      +String path
    }

    User "1" *--> "1" Account
    User "1" *--> "N" Feature
    User "1" *--> "N" Card
    User "1" *--> "N" News
```
