# Next.js + Jest
## How to Use

Execute [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) with [npm](https://docs.npmjs.com/cli/init), [Yarn](https://yarnpkg.com/lang/en/docs/cli/create/), or [pnpm](https://pnpm.io) to bootstrap the example:

```bash
npx create-next-app --example with-jest with-jest-app
```

```bash
yarn create next-app --example with-jest with-jest-app
```

```bash
pnpm create next-app --example with-jest with-jest-app
```

## Running Tests

```bash
npm test
```

```bash
yarn test
```

```bash
pnpm test
```

## Branches

* `main` : branche de prod
* `integration` : branche de tests
* `develop` : branche de développement
* `feature/xxx` : branches temporaire pour développer de nouvelles features

## Structure du Pipeline CI/CD

Notre pipeline est divisé en trois grandes étapes :

### Étape "Build"

* **Installation des dépendances** : Gestion des packages npm
* **Analyse de code** : Vérifications statiques et linting
* **Cleaning et Packaging** : Construction de l'application Next.js

### Étape "Tests"

* **Tests unitaires**
* **Tests d'intégration**
* **Tests de régression**
* **Tests de performance**
* **Tests de sécurité**
* **Tests de compatibilité**
* **Tests d'accessibilité**

### Étape "Deploy"

* **Préparation de l'environnement**
* **Déploiement de l'application**
* **Tests de vérification**
* **Tests de validation fonctionnelle**
* **Tests de charge**
* **Déploiement final**
* **Surveillance et monitoring**

## Workflows par branche

* **Liste des branches**
Voici la liste des branches présentes dans le CI/CD, nous pouvons bien constater qu'il y a 4 branches;
- Main
- Integration
- Develop
- feature/test-feature
![Pipeline CI/CD branch list](/images/branches.png)
* **Pipeline "develop"**
Voici la branche develop et comment les commits agissent sur l'environnement de dev.
![Pipeline CI/CD develop branch](/images/passdev.png)
La pipeline de develop
![Pipeline CI/CD develop branch](/images/devpipelinefinal.png)
* **Pipeline "feature"**
![Pipeline CI/CD feature branch](/images/features.png)
* **Pipeline "integration"**
![Pipeline CI/CD integration branch](/images/integration.png)
![Pipeline CI/CD integration branch](/images/integration2.png)
* **Pipeline "main"**
![Pipeline CI/CD main branch](/images/mainpipeline.png)
![Pipeline CI/CD main branch](/images/mainpipeline2.png)