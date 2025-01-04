```mermaid

graph TD;
    A((Start)) --> B[/Input Number of Students/]
    B --> C{Valid Number?}
    C -->|No| D[/Invalid Number/]
    D --> A
    C -->|Yes| E[Collect Student Data]

    E --> F[Calculate Daily Averages]
    F --> G[Main Menu]

    G -->|Add Student| H[Add Student Details]
    G -->|Delete Student| I[Delete Student by ID]
    G -->|Edit Student| J[Edit Student Details]
    G -->|Search Student| K[Search by Name/ID]
    G -->|Print Records| L[Display All Records]
    G -->|Sort Records| M[Sort by Name/ID]
    G -->|Exit| N((End))

    H --> G
    I --> G
    J --> G
    K --> G
    L --> G
    M --> G
