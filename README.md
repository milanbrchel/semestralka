## About project
- Semestrální práce předmětu 4IT572

## Instruction
- Pipeline bude rozdělena na dvě větve. Pokud commitnu kód do nějaké branche, sestaví se mi eshop, otestuje a povolí mi mergnout kód do masteru. Pokud neprojde, bude merge blokován. V okamžiku merge do masteru se spustí workflow, které kromě kroků z předchozího scénáře ještě nasadí eshop pomocí Ansible na EC2.  To jestli použijete vlastní implementaci Dockeru (preferované), nebo již nějaký hotový nechám na vás. Pro jednoduchost může každá pipeline vytvářet novou instanci v EC2, ale po úspěšném nasazení musí starou běžící instanci smazat. 
- Na vypracování projektu máte 14 dní tj. do 22.12., projekty budete odevzdávat v gitovém repozitáři. Link na repo, screenshot nastavení gitového gitového repozitáře pro blokování mergnutí do masteru a screenshot běžícího eshopu mi pošlete buď emailem, nebo soukromou zprávou na Slacku. Samozřejmě dřivější odevzdání je možné.

## Installation Guide
- Install GIT - https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
- Install Docker - https://www.docker.com/products/docker-desktop

## Build/Run
- Source code of the React app is based on "react-shopping-cart" app made under MIT license by Jefferson Ribeiro

#### Requirements

- Node.js
- NPM

```javascript

/* First, Install the needed packages */
npm install

/* Then start both Node and React */
npm start

/* To run the tests */
npm run test

/* Build sources */
npm run build

/* Running e2e tests */
npm run wdio

/* Deploy to Firebase */
./node_modules/.bin/firebase deploy --token=$FIREBASE_DEPLOY_TOKEN


```

## About tests .

- Unit tests
  - All components have at least a basic smoke test
- Integration tests
  - Fetch product and add to cart properly
- e2e
  - Webdriverio - Add and remove product from cart

### Copyright and license

The MIT License (MIT). Please see License File for more information.

Try to trigger2
