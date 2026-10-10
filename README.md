Projeto para desenvolver um projeto usando a aws
## DIAGRAMA DE CLASSES
--- mermaid
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
    Account --> News

---
