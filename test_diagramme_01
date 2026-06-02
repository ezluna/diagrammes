## Diagramme du flux

```mermaid
flowchart LR
    A[Demande affaire] --> B[Analyse PO]
    B --> C{Valeur ?}
    C -->|Non| D[Rejet]
    C -->|Oui| E[Validation données]
    E --> F{Données dispo ?}
    F -->|Non| G[Attente]
    F -->|Oui| H[Analyse TI]
    H --> I{Faisable ?}
    I -->|Non| J[Re-cadrage]
    I -->|Oui| K[Backlog]
    K --> L[Livraison]
