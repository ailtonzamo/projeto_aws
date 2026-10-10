Projeto para desenvolver um projeto usando a aws
## 📊 Diagrama de Classes

```mermaid
classDiagram
    class Account {
        +String name
        +String accountNumber
        +String accountAgency
        +Float accountBalance
        +Float accountLimit
    }

    class Pix {
        +String pixIcon
        +String pixDescription
    }

    class Pay {
        +String payIcon
        +String payDescription
    }

    class Transfer {
        +String transferIcon
        +String transferDescription
    }

    class Card {
        +String cardNumber
        +Float cardLimit
    }

    class News {
        +String newsIcon
        +String newsDescription
    }

    Account --> Pix
    Account --> Pay
    Account --> Transfer
    Account --> Card
    Account --> News
    Users "1" -- "1" Account
    Users "1" -- "N" Transfer
    Users "1" -- "1" Card
    Users "1" -- "N" News

