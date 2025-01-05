```mermaid
flowchart TD
    A((Start)) --> B[/Input number of students/]
    B -->|Valid| C[Collect student data]
    C --> D[/Input student name/]
    D -->|Valid| E[/Input student ID/]
    E -->|Valid| F[/Input daily study hours/]
    F --> G[Calculate total study hours]
    G --> H[Calculate daily averages]
    H --> I[/Display menu/]
    
    I --> J[Add Student]
    I --> K[Delete Student]
    I --> L[Edit Student]
    I --> M[Search Student]
    I --> N[Print all records]
    I --> O[Sort records]
    I --> P[/Exit/]

    J --> C
    K --> Q[/Enter ID to delete/]
    Q -->|Found| R[Delete student]
    R --> I
    Q -->|Not Found| I

    L --> S[/Enter ID to edit/]
    S -->|Found| T[Edit student details]
    T --> I
    S -->|Not Found| I

    M --> U[/Search for student/]
    U -->|Found| V[/Display student details/]
    U -->|Not Found| I

    N --> W[/Display all records/]
    W --> I

    O --> X[/Sort by Name or ID/]
    X --> I

    P --> Z((End))
