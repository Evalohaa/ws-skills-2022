# Docker

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la création d'une image docker ✔️
   Il y a deux mpyens d'obtenir une image, soit on la buid soit nous la cherchons sur Dockerhub
  
- l'éxécution d'un container ✔️ 
  Un container est une instance d'une image
  On peut lancer pleins de containers avec une image
  
- l'orchestration de containers avec docker-compose ✔️
  docker-compose.yml permet d'écrire les actions à réaliser afin de démarrer une applications composée de différents containers
  docker compose -f docker-compose.dev.yml up (lorsque l'on souhaite démarrer les containers)
  docker compose -f docker-compose.dev.yml build (lorsqu'il y a des images qui ont changé)
  


## 💻 J'utilise

  - Dockerhub pour hoster mes images (si je souhaite les avoir en ligne)

### Un exemple personnel commenté ❌ / ✔️
docker-compose.yml
services:
    server:
        build: ./server
        ports: 
            - 5050:5000
        command: npm run dev
        volumes: 
            - ./server/src/:/app/src/
    mongodb:
        image: mongo
        volumes: 
            - ./data:/data/db

### Utilisation dans un projet ❌ / ✔️

[lien github](...)

Description :

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
