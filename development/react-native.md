# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les différences et points communs entre du code react et du code react native ✔️
- ce que devient et comment est interprêté le code javascript dans une application react native ✔️
- les avantages et inconvénients de react native  ✔️
- la différence entre react native et expo  ✔️
- les principales briques qui composent react native (core components)  ✔️
- comment écrire du style en react native  ✔️
- comment est géré le layout en react native ✔️

## 💻 J'utilise

### Un exemple personnel commenté  ✔️

```
//components/Projects.tsx: affiche la liste des projets sous forme de liste grâce à FlatList
//La liste est scrollable horizontalement, et chaque projet est affiché grâce au composant ProjectCard.
//Les données sont envoyées dans le composant ProjectCard grâce à la props data.
//La props data est un tableau d'objets, chaque objet contient les informations d'un projet.
//renderItem permet de définir le rendu de chaque élément de la liste de projets.
//TouchableOpacity permet de rendre le composant cliquable.
//onPress permet de naviguer vers la page de détails d'un projet en cliquant sur un projet.

    <FlatList
      data={allUserProjects}
      horizontal={true}
      showsVerticalScrollIndicator={false}
      keyExtractor={(item) => item.id.toString()}
      refreshing={refreshing}
      onRefresh={handleRefresh}
      renderItem={({ item }) => (
        <TouchableOpacity
          onPress={() =>
            navigation.navigate('Project_details', {
              projectId: item.id,
              
            })
          }
        >
          <ProjectCard
            id={item.id}
            title={item.title}
            subject={item.subject}
            createdAt={item.createdAt}
            tickets={item.tickets}
          />
        </TouchableOpacity>
      )}
    />
```

### Utilisation dans un projet  ✔️

[https://github.com/WildCodeSchool/structure-mobile](...)

Description : Projet de groupe, application mobile de gestion de projets.

### Utilisation en production si applicable❌ 

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ 

Description :

## 🌐 J'utilise des ressources

### Titre

- https://docs.expo.dev/ : documentation officielle de expo
- https://reactnative.dev/docs/0.70/components-and-apis : documentation officielle de react native

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description: Comment connecter l'application à la base de données ?

Plan d'action : (à valider par le formateur)

- Lancer l'application back-end ❌ / ✔️
- Installer Apollo Client ❌ / ✔️
- Créer un pont HTTP ❌ / ✔️

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
