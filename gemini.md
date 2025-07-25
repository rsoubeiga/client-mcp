# Contexte du projet Client MCP

## Description
Ceci est une application Spring Boot multi-modules implémentant une architecture hexagonale avec une séparation claire entre la logique métier (module `application`) et les adapters d'infrastructure (module `infrastructure`).

## Conventions
- Utilisation de Java 21
- Architecture hexagonale
- Spring Boot 3.5.4
- Lombok pour réduire le boilerplate
- MapStruct pour le mapping d'objets
- Utilisation des gitmojis dans les messages de commit

## Modules
- `application`: Contient la logique métier et les ports
- `infrastructure`: Contient les adapters (REST, persistence) et les dépendances externes

## Attentes pour la génération de code
- Suivre les conventions Spring Boot
- Utiliser Lombok pour les getters/setters/constructeurs
- Implémenter les mappers avec MapStruct quand nécessaire
- Créer des tests unitaires avec JUnit
- Suivre les principes de l'architecture hexagonale

## Structure des packages
- `com.rod.clientmcp`: Module principal
- `com.rod.application`: Module contenant la logique métier
- `com.rod.infrastructure`: Module contenant les adapters d'infrastructure

## Dépendances principales
- Spring Boot Starter Web (pour les APIs REST)
- Spring Boot Starter Data JPA (pour la persistance)
- Spring Boot Starter WebSocket (pour les communications en temps réel)
- H2 Database (base de données en mémoire pour le développement)
- Lombok (pour réduire le code boilerplate)
- MapStruct (pour le mapping objet-objet)

## Conventions de commit
- Utilisation de gitmojis pour catégoriser les commits
- Messages de commit et titres en anglais
- Format: `:<gitmoji> <message>`