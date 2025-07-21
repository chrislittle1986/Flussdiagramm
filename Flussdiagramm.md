
    A[Start: Handy Akkustand prüfen] --> B{Ist der Akkustand unter 20%?}
    
    B -->|Ja| C[Sofort aufladen!]
    B -->|Nein| D{Ist der Akkustand unter 50%?}
    
    D -->|Nein| E[Nicht aufladen nötig]
    D -->|Ja| F{Habe ich heute noch viel vor?}
    
    F -->|Nein| G[Kann warten bis später]
    F -->|Ja| H{Ist eine Steckdose in der Nähe?}
    
    H -->|Nein| I{Habe ich ein Powerbank dabei?}
    H -->|Ja| J[Jetzt aufladen]
    
    I -->|Nein| K{Werde ich länger als 4 Stunden unterwegs sein?}
    I -->|Ja| L[Mit Powerbank aufladen]
    
    K -->|Ja| M[Steckdose suchen und aufladen]
    K -->|Nein| N[Akku reicht wahrscheinlich]
    
    C --> O[Ende]
    E --> O
    G --> O
    J --> O
    L --> O
    M --> O
    N --> O
    
    style C fill:#ff9999
    style J fill:#99ff99
    style L fill:#99ff99
    style M fill:#99ff99
    style E fill:#ffff99
    style G fill:#ffff99
    style N fill:#ffff99
