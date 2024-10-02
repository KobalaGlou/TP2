# Documentation GitFlow de base

## Introduction
GitFlow est une stratégie de gestion de branches dans Git, popularisée par Vincent Driessen. Elle permet de mieux organiser les workflows de développement, en séparant le travail en plusieurs types de branches.

## Branches principales

### 1. `main`
- Contient le code en production.
- Doit toujours être stable.
- Les versions finales du projet y sont fusionnées.

### 2. `develop`
- Contient la dernière version de développement du projet.
- Reçoit les fonctionnalités terminées et testées.

## Branches de support

### 3. `feature/*`
- Branche utilisée pour développer une nouvelle fonctionnalité.
- Créée à partir de `develop` et fusionnée dans `develop` une fois terminée.
  
  ```bash
  git checkout develop
  git checkout -b feature/nom-fonctionnalité
