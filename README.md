# Gestion des tâches — Projet CI/CD

## 📌 Présentation

Ce projet consiste à développer une API REST de gestion des tâches avec **Java et Spring Boot**, puis à mettre en place un pipeline CI/CD avec **Jenkins**.

L'objectif est d'apprendre à utiliser Git et GitHub pour gérer le code source et à automatiser les tests et la compilation du projet.

## 🎯 Objectifs

- Utiliser Git pour suivre les modifications du code.
- Héberger le projet sur GitHub.
- Comprendre les bases de Maven.
- Automatiser les tests avec Jenkins.
- Automatiser la compilation et la génération du fichier JAR.
- Comprendre les étapes d'un pipeline CI/CD.
- Découvrir le fonctionnement d'un `Jenkinsfile`.

## 🛠️ Technologies utilisées

| Technologie | Rôle |
|---|---|
| Java 21 | Langage de programmation |
| Spring Boot | Développement de l'API REST |
| Maven | Gestion des dépendances et compilation |
| Git | Gestion des versions |
| GitHub | Hébergement du code source |
| Jenkins | Automatisation du pipeline CI/CD |
| MySQL | Base de données de l'application |
| H2 | Base de données utilisée pour les tests |

## ⚙️ Prérequis

Avant de lancer le projet, il faut installer :

- JDK 21
- Git
- Maven, ou utiliser le Maven Wrapper fourni avec le projet
- MySQL
- Jenkins pour exécuter le pipeline CI/CD

## 🚀 Installation et lancement

### 1. Cloner le projet

```bash
git clone https://github.com/takoua-khedhri/gestion-taches.git
cd gestion-taches
```

### 2. Configurer la base de données

Créer une base de données MySQL nommée `gestion_taches`.

Configurer les identifiants de connexion dans le fichier local `local.properties`, selon la configuration de l'application.

**Important :** ne jamais publier les identifiants de la base de données sur GitHub.

### 3. Lancer les tests

Sous Windows :

```bat
mvnw.cmd test
```

### 4. Compiler le projet et générer le fichier JAR

```bat
mvnw.cmd package
```

Le fichier JAR généré se trouve normalement dans le dossier `target/`.

## 🔄 Pipeline CI/CD avec Jenkins

Le pipeline Jenkins automatise plusieurs étapes :

1. **Vérification** : afficher un message pour confirmer le démarrage du pipeline.
2. **Récupération du code** : télécharger le code depuis GitHub.
3. **Tests** : exécuter les tests automatisés avec Maven.
4. **Compilation et packaging** : compiler le projet et générer le fichier JAR.

Le pipeline permet de détecter plus rapidement les erreurs et de vérifier que le projet peut être compilé.

## 📚 Compétences acquises

À travers ce projet, je développe mes compétences en :

- Git et GitHub
- Java et Spring Boot
- Maven
- Tests automatisés
- Jenkins et pipelines CI/CD
- Automatisation du processus de développement

## 👩‍💻 Auteur

**Takoua Khedhri**

Projet personnel d'apprentissage DevOps — Git, CI/CD et Jenkins.
