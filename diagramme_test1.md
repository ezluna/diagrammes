## Cas d’usage IA — Priorisation

### 🎯 Objectif
Structurer la décision d’intégrer un cas d’usage IA dans le backlog.

---

### 🔷 Flux produit

1. Demande affaire  
2. Analyse valeur PO  
3. Décision de priorisation  
4. Validation des données  
5. Analyse de faisabilité TI  
6. Intégration backlog  
7. Livraison  

---

### 🔷 Logique décisionnelle

- Si valeur faible → rejet  
- Si données indisponibles → dépendance  
- Si faisabilité TI faible → re-cadrage  

---

### 🔷 Zones

| Zone | Responsable |
|------|------------|
| Produit | PO |
| Données | Data |
| TI | Tech |

---

### 🔷 Diagramme (source — Mermaid)

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
