# L1 — Périmètre TFI
**Prévu : 24 août 2026**

---

## 🎯 Portée de l’initiative

Les travaux de l’entrepôt Paiement Sans Carte portent principalement sur le **volet analytique** :

- Prise de besoins d’affaires  
- Valorisation des données  
- Conception de cas d’usage analytiques  

👉 Le volet analytique constitue la **portée actuelle de l’initiative**

---

## 1. Solution couverte

- Transferts de fonds internationaux (TFI)

❗ Aucune autre solution de paiement sans carte n’est incluse au L1

---

## 2. Sources de données couvertes

### Sources principales

- **API‑TFE**  
  → Données transactionnelles courantes (historique 4–5 ans)

- **PEGA (Smart Investigate)**  
  → Données opérationnelles et d’investigation  

- **FlexCube**  
  → Données historiques liées aux TFI  

### Couverture

Ces sources couvrent :

- Données courantes  
- Données historiques  

---

## 3. Cas d’usage

### Objectifs

Les cas d’usage visent à :

- Améliorer l’autonomie des équipes produit  
- Réduire le temps de préparation des données  
- Améliorer la prise de décision  
- Renforcer la vigie opérationnelle  

👉 La priorisation est basée sur la **valeur d’affaires**

---

## 4. Arrimage avec les équipes consommatrices

### Utilisateurs identifiés

| Type d’utilisateur | Rôle |
|------------------|------|
| Responsables produit TFI | Pilotage de la performance, décisions d’optimisation |
| Conseillers processus TFI | Analyse des délais, volumétrie et amélioration continue |
| Utilisateurs analytiques transverses | Analyses globales (ex. Vue 360) |

---

### Modalités d’arrimage

- Communication régulière sur l’avancement  
- Partage structuré de la disponibilité des données  
- Alignement sur les besoins analytiques  

---

## 5. Fondation de données

### Composantes clés

- Ingestion des données  
- Structuration granulaire (niveau transactionnel)  
- Historisation des données  
- Application de règles de transformation  
- Gouvernance et qualité des données  

### Livraison

👉 Mise à disposition des données dans la **PDM pour consommation analytique**

---

## 6. Modèle de données

### Objectifs

Le modèle vise à :

- Structurer les données de manière cohérente et granulaire  
- Permettre la réutilisation multi-usages  
- Garantir la cohérence des indicateurs  

---

## 7. Domaines de valeurs et mapping

### Contexte

Les indicateurs reposent sur des **dimensions clés** :

- Canal  
- Direction  
- Type de transaction  
- etc.

---

### Enjeu

Un travail de mapping est requis pour :

- Aligner les valeurs provenant des différentes sources  
- Définir un domaine de valeurs cible unifié  
- Gérer les écarts entre :
  - modèle actuel (CMP)
  - modèle cible (PSC)

---

### Principes

Les domaines de valeurs doivent être :

- Clairs  
- Homogènes  
- Partagés entre les équipes  

---

## 8. Règles d’affaires et de transformation

### Règles d’affaires

Définissent :

- Indicateurs  
- Dimensions  
- Classifications  

---

### Règles de transformation

Permettent de :

- Reconstruire les indicateurs cibles  
- Normaliser les données sources  
- Assurer la cohérence entre systèmes  

---

## 9. Gestion des données (historique et courant)

### Objectif

Assurer la **cohérence entre données historiques et courantes**

---

### Sources couvertes

- Flux courants → API‑TFE  
- Historique → FlexCube  

---

### Décision requise

Définir :

- La stratégie de gestion de l’historique  
- La re-application ou non des transformations  

---

## 10. Séquencement des travaux

### Étapes

1. Production des besoins d’affaires  
2. Priorisation des indicateurs TFI  
3. Finalisation du mapping (domaines de valeurs)  
4. Documentation de l’existant (CMP)  
5. Définition des règles de transformation  
6. Unification des données historiques et courantes  
7. Implémentation de la modélisation  
8. Accès aux espaces de travail PDM  

---

## 🚫 Hors portée

Les éléments suivants ne sont pas inclus :

- Migration ou reconduction des rapports BI  
- Décommissionnement du CMP  
- Données opérationnelles non analytiques  
- Support des solutions BI des équipes  
- Analyses ad hoc ponctuelles  
- Substitution aux rôles BI, analytiques ou produit
