# 💱 ApiCurrency

**ApiCurrency** est une API facile à utiliser qui fournit des informations de conversion de devises en temps réel. Il utilise des technologies comme Axios, Node.js (Express) et TypeScript.

## Fonctionnalités

- **Conversion Simple** : Obtenez la conversion actuelle d'une devise par rapport à l'euro.
- **Info Monnaie** : Obtenez des informations détaillées sur une devise spécifique.
- **Conversion Datée** : Obtenez la conversion historique d'une devise par rapport à l'euro pour une date donnée.

## Installation

1. **Cloner le Dépôt** :

   ```bash
   git clone https://github.com/ismaa2k/Project_API.1-B2
   cd project_api-doc
   ```

2. **Initialiser TypeScript** :

   ```bash
   npx tsc --init
   ```

3. **Installer les Dépendances** :

   ```bash
   npm install express axios
   npm install --save-dev typescript ts-node @types/express
   ```

4. **Ajouter "start" dans "scripts" dans le `package.json`** :

   ```json
   "scripts": {
     "start": "nodemon --exec ts-node server.ts"
   }
   ```

5. **Démarrer le Serveur** :

   ```bash
   npm start
   ```

## Utilisation

### Exemple d'Utilisation de l'API

Pour obtenir les taux de change actuels ou des informations sur une devise spécifique, utilisez les routes suivantes :

- `/latest/:currency` pour obtenir la conversion actuelle par rapport à l'euro.
- `/info/:currency` pour obtenir des informations détaillées sur une devise spécifique.

**Remarque : Utilisez les abréviations standard des devises, par exemple EUR pour l'euro, USD pour le dollar américain, etc.**

### Avec Postman

Pour tester l'API, vous pouvez utiliser [Postman](https://www.postman.com/downloads/). Configurez simplement votre requête et pointez vers `http://localhost:3000/latest/USD` pour tester la conversion ou vers `http://localhost:3000/info/RUB` pour obtenir des informations sur la devise.

### Avec Swagger

Pour tester l'API avec Swagger, démarrez le serveur avec `npm start`. Puis allez sur l'url : `http://localhost:3000/api-docs`

## Structure du Projet

```plaintext
project_api-doc/
│
├── node_modules/
│
├── public/
│   ├── image.png
│   ├── image-1.png
│   ├── image-2.png
│
├── src/
│   ├── CurrencyController.ts
│   ├── server.ts
│   ├── swaggerOptions.ts
│
├── .gitignore
├── package-lock.json
├── package.json
├── tsconfig.json
└── README.md
```

## Technologies Utilisées

- **Express** : Pour le serveur HTTP.
- **Axios** : Pour effectuer des requêtes HTTP vers des APIs externes.
- **TypeScript** : Pour le typage statique.
- **ts-Node** : Pour exécuter directement le code TypeScript dans Node.js.

---

Voilà **ApiCurrency** ! Si vous avez des questions ou des suggestions, n'hésitez pas à les partager. 🌍✨
