```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : has
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER {
        string name
        string address
    }
    ORDER {
        int order_number
        date date
    }
    LINE-ITEM {
        int quantity
        double price
    }
```