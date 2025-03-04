# Smart-Email-Segmentation-API


Smart Email Segmentation API

📌 Description

Smart Email Segmentation API est une API REST avancée conçue pour analyser l'engagement des utilisateurs dans les campagnes e-mail et les segmenter intelligemment. Elle permet d'automatiser le suivi des interactions et d'améliorer le ciblage marketing en offrant une gestion efficace des segments d'utilisateurs.

🚀 Fonctionnalités

🔹 Suivi des interactions e-mail : Analyse en temps réel des ouvertures et des clics.

🔹 Segmentation automatique : Attribution dynamique des tags "Actifs", "À relancer", "Perdus" en fonction de l'engagement.

🔹 Gestion flexible des segments : Création, mise à jour et suppression des segments personnalisés.

🔹 Intégration avec des plateformes externes : Synchronisation avec Mailchimp, SendGrid, Brevo.

🔹 Tableau de bord analytique : Statistiques détaillées et suivi des performances en temps réel.

🔹 Scalabilité et optimisation : Utilisation de RabbitMQ pour la gestion des événements, cache Redis, et exécution cloud via AWS Lambda.

🛠️ Technologies utilisées

Langage : Java 17

Framework : Spring Boot (Spring Data JPA, Spring Security, Spring Cloud, Spring WebFlux)

Base de données : PostgreSQL / MongoDB

Sécurité : OAuth2, JWT, chiffrement des données sensibles

Messagerie : RabbitMQ / Kafka pour la gestion des événements asynchrones

Cloud & Conteneurisation : AWS Lambda, Docker, Kubernetes

Monitoring : Prometheus, Grafana

📥 Installation

📌 Prérequis

Java 17+

Maven

Docker (pour exécuter PostgreSQL et RabbitMQ)

📌 Étapes d'installation

Cloner le projet

git clone https://github.com/votre-repo/smart-email-segmentation.git
cd smart-email-segmentation

Configurer la base de données (PostgreSQL via Docker)

docker-compose up -d

Configurer les variables d'environnement (Créer un fichier .env et renseigner les valeurs nécessaires)

Lancer l'application

mvn clean install
mvn spring-boot:run

🔗 Endpoints principaux

Méthode

URL

Description

GET

/api/users/{id}

Récupérer un utilisateur

POST

/api/segments

Créer un segment

PUT

/api/segments/{id}

Mettre à jour un segment

DELETE

/api/segments/{id}

Supprimer un segment

GET

/api/analytics

Obtenir les statistiques

☁️ Déploiement

📌 Déploiement avec Docker

docker build -t smart-email-api .
docker run -p 8080:8080 smart-email-api

📌 Déploiement sur AWS Lambda

Utilisation de AWS SAM ou Serverless Framework

Définition des functions Lambda pour le traitement des événements asynchrones

🧪 Tests

mvn test

🤝 Contributions

Les contributions sont les bienvenues ! Merci de soumettre une issue ou une pull request pour toute amélioration ou correction.
