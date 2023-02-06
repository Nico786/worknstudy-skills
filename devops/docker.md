# Docker

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la création d'une image docker  ✔️
- l'éxécution d'un container  ✔️
- l'orchestration de containers avec docker-compose  ✔️


## 💻 J'utilise

### Un exemple personnel commenté  ✔️

```
//Création d'une image docker pour le projet front

FROM node:lts

RUN mkdir /app
WORKDIR /app
COPY package*.json ./
RUN npm i
RUN npm i -g typescript ts-node-dev 
COPY src src
COPY tsconfig.json tsconfig.json
COPY prisma prisma
```

### Utilisation dans un projet ❌ / ✔️

[https://github.com/WildCodeSchool/2203-wns-etchebest-tfs-back](...)

Description :

### Utilisation en production si applicable ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ✔️

Description : Oui, j'utilise docker dans mon entreprise

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
