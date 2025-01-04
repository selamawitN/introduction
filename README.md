```mermaid
graph TD
    A[Start] --> B[/Enter number of students/]
    B --> C{Validate number of students}
    C -- Yes --> D[/Input student data/]
    C -- No --> E[/Invalid input message /]
    D --> F[Calculate daily averages]
    F --> G[Display Menu]
    G --> H{Choose option}
    H --> I[Add student]
    H --> J[Delete student]
    H --> K[Edit student]
    H --> L[Search student]
    H --> M[Print records]
    H --> N[Sort records]
    H --> O[Exit]
    I --> D
    J --> D
    K --> D
    L --> D
    M --> D
    N --> D
    E --> O
    O --> P[End]
