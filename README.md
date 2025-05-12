# 🧪 TP DevOps – Intégration de SonarQube avec Jenkins via Docker

## 🎯 Objectif

Ce projet vise à mettre en place une **chaîne d'intégration continue (CI)** en utilisant **Jenkins** et **SonarQube**, conteneurisés avec **Docker**, afin d’automatiser l’analyse de la qualité du code source d’un projet hébergé sur Git.

---

## 🛠️ Outils utilisés

| Outil         | Version                 | Rôle                                                      |
|---------------|-------------------------|-----------------------------------------------------------|
| Docker        | Latest                  | Conteneurisation des services Jenkins et SonarQube        |
| Jenkins       | jenkins/jenkins:latest  | Serveur d'intégration continue                            |
| SonarQube     | sonarqube:latest        | Analyse statique et qualité du code                       |
| Git           | N/A                     | Versionnement du code source                              |
| Navigateur Web| N/A                     | Accès aux interfaces de Jenkins et SonarQube              |

---

## 📋 Prérequis

- Docker et Docker Compose installés
- Connexion Internet active
- Connaissances de base en Git
- Un projet de code source à analyser

---

## 🚀 Étapes du projet

### 1. Création de l’environnement Docker
- Téléchargement des images Docker de Jenkins et SonarQube
- Création d’un réseau Docker partagé
- Lancement des conteneurs via `docker-compose`

### 2. Configuration de Jenkins
- Installation des plugins :
  - *SonarQube Scanner*
  - *SonarQube Quality Gates*
- Ajout et configuration du Scanner dans Jenkins

### 3. Configuration de SonarQube
- Création d’un utilisateur admin
- Génération d’un token d’authentification pour Jenkins

### 4. Intégration Jenkins ↔ SonarQube
- Configuration des identifiants dans Jenkins
- Ajout du serveur SonarQube dans la section “Global Tool Configuration”

### 5. Mise en place du pipeline CI
- Création d’un job de type Pipeline dans Jenkins
- Connexion au dépôt Git contenant le code
- Définition du `Jenkinsfile` pour inclure l’analyse SonarQube

### 6. Analyse du code
- Exécution manuelle ou automatisée du pipeline
- Résultats analysés sur SonarQube : bugs, code smells, duplications, etc.

---

## 📈 Résultats et qualité

- Analyse statique automatisée via Jenkins et SonarQube
- Détection de problèmes de qualité et sécurité
- Amélioration continue basée sur les rapports SonarQube

---

## 📚 Ressources supplémentaires

- [Documentation Jenkins](https://www.jenkins.io/doc/)
- [Documentation SonarQube](https://docs.sonarsource.com/)
- [Docker Hub - Jenkins](https://hub.docker.com/r/jenkins/jenkins)
- [Docker Hub - SonarQube](https://hub.docker.com/_/sonarqube)

---

## ✍️ Réalisé par

**IMASSENDA Salma**  
Encadré par **Pr. RABHI**

---

## 📎 License

Projet académique – réservé à un usage pédagogique uniquement.
