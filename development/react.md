# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'état (_state_) pour contrôler l'affichage d'un composant ✔️
- les composants enfants et les _props_ qu'on leur passe  ✔️
- le déclenchement d'instructions en fonction des actions de l'utilisateur ✔️
- le déclenchement d'instructions en fonction de l'étape du cycle de vie du composant ou du changement de valeur de ses props ✔️
- l'usage d'un reducer (_useReducer_) pour gérer un état composé dans un composant ❌ 
- l'état stocké dans un composant avec un _context provider_ et accessible dans ses descendants via `useContext` ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```
// Récupération des projets de l'utilisateur, avec le hook useQuery de react-query
// useQuery permet de récupérer les données d'une requête GraphQL
// handleRefresh permet de rafraichir la liste des projets, en appelant la fonction refetch de useQuery
// setProjects permet de mettre à jour la liste des projets
// useEffect permet de rafraichir la liste des projets à chaque fois que le state data est modifié

  const handleRefresh = () => {
    setRefreshing(true);
    refetch();
    setRefreshing(false);
  };

  useEffect(() => {
    handleRefresh();
    setProjects(allUserProjects);
  }, [data]);

```

### Utilisation dans un projet ✔️

[https://github.com/Nico786/oners]

Description : site vitrine pour une bd "webtoon" - en cours


### Utilisation en production si applicable❌ 

[https://oners-demo.herokuapp.com]

Description : site vitrine pour une bd "webtoon" - en cours

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Titre

- https://nextjs.org/docs: documentation NextJS
- https://react-query.tanstack.com/overview: documentation react-query
- https://fr.reactjs.org/docs/getting-started.html : documentation ReactJS

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
