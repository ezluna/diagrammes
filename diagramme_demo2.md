## Flux Data — Chaîne analytique simplifiée

### 🎯 Objectif
Modéliser un flux de données complet allant des sources opératoires jusqu’à la consommation analytique.

---

### 🔷 Vue d’ensemble

Pipeline structuré en 4 couches :
- Sources
- Ingestion
- Valorisation
- Consommation

---

### 🔷 Acteurs

| Domaine | Rôle |
|--------|------|
| Produit | Définit les besoins et priorités |
| Data | Gère ingestion, qualité et transformation |
| TI | Assure l’infrastructure et la livraison |

---

### 🔷 Étapes du pipeline

#### Sources
- Applications métiers
- APIs externes
- Données historiques

#### Ingestion
- Zone brute (raw)
- Zone nettoyée (clean)
- Zone enrichie

#### Valorisation
- Construction des modèles
- Règles de transformation
- Agrégation des indicateurs

#### Consommation
- Tableaux de bord
- Rapports
- Services analytiques

---

### 🔷 Diagramme global (architecture)

```mermaid
flowchart LR

%% SOURCES
subgraph Sources
    S1[Applications métiers]
    S2[APIs externes]
    S3[Données historiques]
end

%% INGESTION
subgraph Ingestion
    I1[Zone brute]
    I2[Zone nettoyée]
    I3[Zone enrichie]
end

%% VALORISATION
subgraph Valorisation
    V1[Modélisation]
    V2[Transformation]
    V3[Indicateurs]
end

%% CONSOMMATION
subgraph Consommation
    C1[BI / dashboards]
    C2[Rapports]
    C3[Services analytiques]
end

%% FLOW
S1 --> I1
S2 --> I1
S3 --> I1

I1 --> I2 --> I3
I3 --> V1 --> V2 --> V3

V3 --> C1
V3 --> C2
V3 --> C3

