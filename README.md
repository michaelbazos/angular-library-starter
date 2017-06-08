# angular-library-starter

This project is an implementation of [Angular Package Format v4.0](https://goo.gl/AMOU5G), so as to build library of components for angular applications. As a consequence, the library can be consumed in various ways, e.g. from apps using Webpack, from apps using SystemJS, from a jsfiddle, a plunkr, etc.

## Features

 - Generation to various module formats: FESM15, FESM5, UMD
 - Type definitions
 - Metadata for AOT compilation

## Getting started

1. Clone the library

  ```sh
  git clone https://github.com/michaelbazos/angular-library-starter.git
  ```
  
2. Install dependencies and build the library

  ```sh
  cd angular-library-starter
  npm install
  npm run build
  ```
  
3. Add the built library as dependency to your application

From your consumer application folder:

  ```sh
  npm install ../angular-library-starter/dist --save
  ```
  
  Adjust the path to the _dist_ folder accordingly.
  
  Note 1: this installation refers to a local folder. Once you're done you should publish your library to a package manager.
  Note 2: Argument `--save` is implicit as of npm5
  
4. Import the library in the application

  ```ts
  import { MylibModule } from 'mylib';
   
  @NgModule({
    declarations: [
      AppComponent
    ],
    imports: [
      ... ,
   
      MylibModule
    ],
    providers: [],
    bootstrap: [ AppComponent ]
  })
  
  export class AppModule { }
  ```

5. Use the components

  ```html
  <ui-dropdown></ui-dropdown>
  ```

## License

MIT © [Michael Bazos](mailto:micabazos@gmail.com)
