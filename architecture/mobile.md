# Technologies d'applications mobiles

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les différences entre les webapps, les applications hybrides et natives ✔️
- le fonctionnement d'une app React Native, ce qui sera en réalité produit et installé sur le téléphone de mes utilisateur·rices, comment le JS arrive à communiquer avec le natif ✔️
- quelles sont les différentes technologies (frameworks) existantes pour développer des apps mobiles ✔️
- quels sont les principaux points d'attention entre le développement d'une app mobile ou desktop  ✔️

## 💻 J'utilise

### Un exemple personnel commenté  ✔️

```
JSX d'un composant React Native affichant une liste de projets, permettant de naviguer vers la page de détails d'un projet en cliquant sur l'élément de la liste:

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
  );
```

### Utilisation dans un projet  ✔️

[https://github.com/WildCodeSchool/structure-mobile](...)

Description : Application de gestion de ticket, développée en React Native et apollo client

### Utilisation en production si applicable ❌ 

[lien du projet](...)

Description : Nous n'avons pas déployé l'application sur le store

### Utilisation en environement professionnel ❌ 

Description : Nous n'avons pas développé d'applications mobiles à mon entreprise

## 🌐 J'utilise des ressources

### Titre

- documentation de expo et react native

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
- J'ai ecrit un [article](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
