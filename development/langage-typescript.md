# TypeScript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer


- l'intéret de TypeScript dans l'IDE ✔️
- les types de bases ✔️
- comment et pourquoi étendre une interface ✔️
- les classes et les decorators ✔️


## 💻 J'utilise

### Un exemple personnel commenté  ✔️
  
```typescript
// Déclaration d'une interface User, spécifiant le type de ses propriétés (email et password doivent être de type string)
interface User {
  email: string;
  password: string;
}

// Définition d'une fonction affichant l'email d'un utilisateur. Cette fonction prend en paramètre un objet de type User
function displayEmail(user: User) {
  console.log(user.email);
}

// Instanciation d'un objet de type User
const userToto: User = {
  email: "toto", // si on met un nombre ici, on aura une erreur car le type de la propriété email est string
  password: "toto",
};

// Appel de la fonction displayEmail avec l'objet userToto en paramètre
displayEmail(userToto);
```

### Utilisation dans un projet  ✔️

[https://github.com/WildCodeSchool/2203-wns-etchebest-tfs-front/](...)

Description : Projet de groupe, application de ticketing - utilisation de TypeScript dans un projet NextJS


### Utilisation en production si applicable ✔️

[https://etchebest-1-04-22.wilders.dev/login](...)

Description : Projet de groupe, instance de staging

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Titre

- https://www.typescriptlang.org/docs/
- documentation officielle de TypeScript

## 🚧 Je franchis les obstacles

### Point de blocage ❌

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌
- action 2 ❌
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌
- J'ai fait une [présentation](...) ❌
