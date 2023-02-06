# Sécurité dans le développement Web

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- Le rôle de l'OWASP  ✔️
- Les injections SQL  ✔️
- XSS  ✔️
- CRSF  ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```
// l'ORM Prisma permet de sécuriser les requêtes SQL en préparant les requêtes avant de les envoyer à la base de données, permettant ainsi de se prémunir des injections SQL

prisma = new PrismaClient();

 const user = await prisma.user.create({
        data: {
          firstname: firstname.trim(),
          lastname: lastname.trim(),
          email: email.trim().toLowerCase(),
          password
      },

```

### Utilisation dans un projet ✔️

[https://github.com/WildCodeSchool/2203-wns-etchebest-tfs-back](...)

Description : Projet de groupe, application de ticketing - utilisation de l'ORM Prisma

### Utilisation en production si applicable ✔️

[https://staging.etchebest-1-04-22.wilders.dev/](...)

Description :

### Utilisation en environement professionnel  ✔️

Description : Utilisation de l'api QuerySet de Django, permettant de sécuriser les requêtes SQL

## 🌐 J'utilise des ressources

### Titre

- https://www.prisma.io/docs
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
