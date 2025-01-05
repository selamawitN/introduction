```mermaid
 

flowchart TD
    A((Start)) --> B[/Input number of students/]
    B -->|Valid| C[Collect student data]
    B -->|Invalid| AE((End))  
    C --> D[/Input student name/]
    D -->|Valid| E[/Input student ID/]
    E -->|Valid| F[/Input daily study hours/]
    F --> G[Calculate total study hours]
    G --> H[Calculate daily averages]
    H --> I[Display menu]
    
    I --> J[Add Student]
    I --> K[Delete Student]
    I --> L[Edit Student]
    I --> M[Search Student]
    I --> N[Print all records]
    I --> O[Sort records]
    I --> P[/Exit/]

    J --> C
    K --> Q[/Enter ID to delete/]
    Q --> R{Is ID found?}
    R -->|Yes| S[/Delete student/]
    S --> I
    R -->|No| T[/Student not found/]
    T --> Q  

    L --> U[/Enter ID to edit/]
    U --> V{Is ID found?}
    V -->|Yes| W[/Edit student details/]
    W --> I
    V -->|No| X[/Student not found/]
    X --> U  

    M --> Y[/Search for student/]
    Y --> Z{Is ID found?}
    Z -->|Yes| AA[/Display student details/]
    Z -->|No| AB[/Student not found/]
    AB --> Y  

    N --> AC[/Display all records/]
    AC --> I

    O --> AD[/Sort by Name or ID/]
    AD --> I

    P --> AE((End))
