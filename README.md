```mermaid
flowchart TD
    A[App Launch] --> B[Splash Screen]
    B --> C[Home Screen]

    C --> D[Choose Math Topic]
    D --> E[Exercise Screen]

    E --> F{Answer Correct?}
    F -- Yes --> G[Positive Feedback]
    F -- No --> H[Hint / Retry]

    G --> I[Update Progress & Streak]
    H --> E

    I --> C

    C --> J[Progress Screen]
    J --> C

    C --> K[Settings Screen]
    K --> C
