# Tester son application

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les tests unitaires ✔️
- les mocks  ✔️
- les tests d'integration  ✔️
- les tests de bout en bout (end to end)  ✔️
- le TDD  ✔️
- les tests par snapshot ❌ 

## 💻 J'utilise

### Un exemple personnel commenté  ✔️

```
Ajout d'un test end to end avec playwright pour vérifier que l'on peut s'inscrire à l'application, que l'on peut se déconnecter, et que l'on peut se connecter à nouveau. Ce code va tester chaque étape de ce scénario.

test.describe("Struture App", ()=>{
  test('Should register then logout then login', async ({ page, browserName }) => {
    await page.goto('http://localhost:3000/register');
    await page.getByPlaceholder('Votre prénom').click();
    await page.getByPlaceholder('Votre prénom').fill('test');
    await page.getByPlaceholder('Votre nom').click();
    await page.getByPlaceholder('Votre nom').fill('test');
    await page.getByPlaceholder('email@exemple.com').click();
    await page.getByPlaceholder('email@exemple.com').fill(`test-${browserName}@test.com`);
    await page.getByPlaceholder('Saisissez votre mot de passe').click();
    await page.getByPlaceholder('Saisissez votre mot de passe').fill('123456789');
    await page.getByPlaceholder('Comfirmez votre mot de passe').click();
    await page.getByPlaceholder('Comfirmez votre mot de passe').fill('123456789');
    await page.getByRole('button', { name: 'S\'inscrire' }).click();
    delay(2000).then(async ()=>{
      await expect(page).toHaveURL('/')
      await page.locator('.absolute').first().click();
      await page.getByRole('button', { name: 'Se déconnecter' }).click();
      await expect(page).toHaveURL('/login')
      await page.getByPlaceholder('email@exemple.com').click();
      await page.getByPlaceholder('email@exemple.com').fill('test50@gmail.com');
      await page.getByPlaceholder('Saisissez votre mot de passe').click();
      await page.getByPlaceholder('Saisissez votre mot de passe').fill('123456789');
      await page.getByRole('button', { name: 'Connexion' }).click();
    })
  });

```

### Utilisation dans un projet ❌ / ✔️

[https://github.com/WildCodeSchool/2203-wns-etchebest-tfs-front](...)

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
