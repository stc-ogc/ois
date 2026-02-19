flowchart TD
    A[User Opens Home Screen] --> B[User Clicks Emoji Button]
    B --> C[JavaScript addEventListener Triggered]
    C --> D[Identify Selected Mood]
    D --> E[Save Mood to LocalStorage]
    E --> F[Retrieve Existing Mood Data]
    F --> G[Update Mood History Array]
    G --> H[Store Updated Array in LocalStorage]
    H --> I[Display Confirmation Message]
    I --> J[Redirect to Recommendations Screen]

