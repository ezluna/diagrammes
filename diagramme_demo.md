## Cas d’usage IA — Priorisation multi-partenaires

### 🎯 Objectif
Structurer un cas d’usage IA impliquant plusieurs parties prenantes (affaires, data, TI) avec des itérations de validation et de livraison.

---

### 🔷 Vision produit

Permettre d’analyser, prioriser et livrer des cas d’usage IA tout en assurant :

- valeur d’affaires démontrée
- données disponibles et fiables
- faisabilité technologique
- alignement avec les partenaires

---

### 🔷 Acteurs

| Acteur | Rôle |
|-------|------|
| Affaires | Exprime le besoin |
| PO | Analyse et priorise |
| Équipe Data | Valide et prépare les données |
| TI | Implémente la solution |

---

### 🔷 Flux utilisateur (simplifié)

1. L’acteur affaires soumet un besoin  
2. Le PO analyse la valeur  
3. Une validation est faite sur les données  
4. Une analyse technologique est réalisée  
5. Le cas est intégré au backlog  
6. Livraison incrémentale  

---

### 🔷 Pipeline de décision

- Si valeur insuffisante → rejet  
- Si données indisponibles → dépendance / attente  
- Si faisabilité TI faible → re-cadrage  
- Sinon → intégration et livraison  

---

### 🔷 Diagramme de contexte

```mermaid
flowchart LR
## Cas d’usage IA — Priorisation multi-partenaires (version avancée)

### 🔷 Diagramme décisionnel (Produit / Data / TI + itérations)

```mermaid
flowchart LR
    A[Demande affaire] --> B[Analyse PO]
    B --> C{Valeur ?}

    C -->|Faible| D[Rejet]
    C -->|Forte| E[Validation données]

    E --> F{Données disponibles ?}
    F -->|Non| G[Attente]
    F -->|Oui| H[Analyse TI]
