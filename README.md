# Simulation de Combustion du Méthane avec DWSIM

## Description
Simulation complète de combustion du méthane avec DWSIM - Modélisation thermodynamique incluant mélangeur air-méthane, réacteur adiabatique et séparation vapeur-liquide. Calculs des bilans matière, analyse des conversions, optimisation procédé industriel. Équation Peng-Robinson pour propriétés thermodynamiques.

## Vue d'ensemble du procédé
Ce projet simule un procédé industriel complet de combustion du méthane comprenant :
- **Mélange des réactifs** : Air et méthane pur
- **Réaction de combustion** : Conversion adiabatique à 25°C
- **Séparation des produits** : Récupération vapeur/liquide

### Réaction chimique
```
CH₄ + 2O₂ → CO₂ + 2H₂O
```

## Caractéristiques techniques

### Conditions opératoires
- **Température du réacteur** : 25°C (adiabatique)
- **Pression** : 1.5 bar
- **Débit massique total** : ~20.75 kg/h
- **Conversion du méthane** : 100%

### Composition des flux
#### Air d'alimentation
- O₂ : 20% molaire
- N₂ : 80% molaire
- Débit : 19.75 kg/h

#### Méthane
- CH₄ : 100% pur
- Débit : 1 kg/h

### Modèle thermodynamique
- **Équation d'état** : Peng-Robinson (PR)
- **Package de propriétés** : Peng-Robinson (PR) (1)

## Structure du procédé

### Équipements simulés
1. **MIX-1** : Mélangeur de flux
   - Inlet 1 : Méthane
   - Inlet 2 : Air
   - Outlet : Mélange réactionnel

2. **RCONV-1** : Réacteur de conversion
   - Mode : Adiabatique
   - Température de sortie : 25°C
   - Conversion O₂ : 90.9%

3. **Séparation** : Unité de séparation vapeur-liquide
   - Produits vapeur et liquide
   - Récupération énergétique

## Résultats de simulation

### Bilans matière
- **Conversion du méthane** : 100%
- **Conversion de l'oxygène** : 90.9%
- **Production de CO₂** : Formation selon stœchiométrie
- **Production de H₂O** : Formation selon stœchiométrie

### Flux de sortie
Les produits de combustion sont séparés en phases vapeur et liquide avec récupération énergétique optimisée.

## Utilisation

### Prérequis
- DWSIM (version compatible)
- Package thermodynamique Peng-Robinson

### Instructions
1. Ouvrir le fichier de simulation DWSIM
2. Vérifier les propriétés des composants
3. Exécuter la simulation
4. Analyser les résultats dans les onglets Results

## Contact et contribution
Ce projet a été développé pour l'étude des procédés de combustion industrielle. Les contributions et améliorations sont les bienvenues.
