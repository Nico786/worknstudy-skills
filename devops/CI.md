# Integration continue

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les enjeux de l'integration continue  ✔️
- la mise en place d'une github action ✔️

## 💻 J'utilise

### Un exemple personnel commenté  ✔️

Création d'un workflow github action pour construire et push une image de prod docker sur le DockerHub, lors d'un push sur la branche main

```
name: Compile and push server image
on:
  push:
    branches: ["main"]
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2

      - uses: docker/login-action@v1
        name: Login to Docker Hub
        with:
          username: ${{ secrets.DOCKER_HUB_USERNAME }}
          password: ${{ secrets.DOCKER_HUB_ACCESS_TOKEN }}

      - uses: docker/setup-buildx-action@v1
        name: Set up Docker Buildx

      - uses: docker/build-push-action@v2
        name: Build and push
        with:
          context: .
          file: ./Dockerfile
          push: true
          tags: ${{ secrets.DOCKER_HUB_USERNAME }}/tfs_deploy_server_prod:latest
```

### Utilisation dans un projet ✔️

[https://github.com/WildCodeSchool/2203-wns-etchebest-tfs-back/actions](...)

Description :

### Utilisation en production si applicable❌ / ✔️

[https://etchebest-1-04-22.wilders.dev/login](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description : Workflow buildant une image docker a chaque PR ouverte sur la branche de production

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
