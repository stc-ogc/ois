```mermaid
flowchart TD
    A[App Launch] --> B[Splash Screen]
    B --> C{First Time User?}

    C -- Yes --> D[Welcome / Intro Screen<br/>Mascot explains app]
    C -- No --> E[Home Screen]

    D --> E

    E --> F[Daily Streak Check<br/>Local Storage]
    F --> G[Display Streak & Progress]

    E --> H[Select Math Topic]
    H --> I[Topic List Screen<br/>Addition / Subtraction / Multiplication / Division]

    I --> J[Difficulty Selection<br/>Easy / Medium / Hard]

    J --> K[Exercise Screen<br/>Question + Mascot Guidance]

    K --> L{Answer Submitted}
    L --> M{Correct?}

    M -- Yes --> N[Positive Feedback Animation<br/>Mascot Praise]
    M -- No --> O[Hint / Explanation<br/>Mascot Encouragement]

    N --> P[Update Score & Progress<br/>Local Storage]
    O --> P

    P --> Q{More Questions?}

    Q -- Yes --> K
    Q -- No --> R[Session Summary Screen<br/>Score / Accuracy / Time]

    R --> S[Update Daily Streak<br/>Local Storage]
    S --> E

    E --> T[Progress Screen]
    T --> U[View Stats<br/>Topics Completed / Accuracy / Streaks]
    U --> E

    E --> V[Settings Screen]
    V --> W[Toggle Sound / Animations / Reset Progress]
    W --> E

    E --> X[Exit App]
