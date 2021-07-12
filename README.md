# lazy-loading-angular
Example project using Lazy Loading in Anguar.

# Default route
![Img1](https://i.imgur.com/yJhcDV7.png)
![Img2](https://i.imgur.com/HZzyON4.png)

# Loading Lazy module
![Img1](https://i.imgur.com/T8mHL0n.png)
![Img2](https://i.imgur.com/8PzOeaY.png)

### Prerequisites
* [Node.js](https://nodejs.org/en/) - Node.js
* [Angular](https://angular.io/) - Angular

### Running
The server can be run locally and also deployed to your own server.

### Run
````
# Install dependencies
npm install

# Run Project
ng serve
````

### As Angular 8+ has introduced the new module loading method, then it is recommended to use:
````
const routes: Routes = [
  ...
  {path: 'lazy', loadChildren: () => import('./lazy/lazy.module').then(m => m.LazyModule)}
];
````

### Authors
* **Lucas Chinarelli** - [chinarelli](https://github.com/Chinarelli)

### Reference
* [Medium](https://medium.com/@thiago.reis/how-to-implement-lazy-loading-in-angular-c8dcbf165561)
* [Angular Docs](https://angular.io/guide/lazy-loading-ngmodules)
