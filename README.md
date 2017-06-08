# angular-library-starter

This project is an implementation of [Angular Package Format v4.0](https://goo.gl/AMOU5G), so as to build library of components for angular applications. As a consequence, the library can be consumed in various ways, e.g. from apps using Webpack, from apps using SystemJS, from a jsfiddle, a plunkr, etc.

## Features

 - Generation to various module formats: FESM15, FESM5, UMD
 - Type definitions
 - Metadata for AOT compilation

## Getting started

1. Install the library

  ```sh
  npm install ui-toolkit --save
  ```
  
Note that `--save` argument is implicit as of npm5.

2. Import it in your application

  ```ts
  // Import the desired module from ui-toolkit library
  import { SampleModule } from 'ui-toolkit';
   
  @NgModule({
    declarations: [
      AppComponent
    ],
    imports: [
      ... ,
   
      SampleModule
    ],
    providers: [],
    bootstrap: [AppComponent]
  })
  
  export class AppModule { }
  ```

3. Use it

  ```html
  <sample-component></sample-component>
  ```

## License

MIT © [Michael Bazos](mailto:micabazos@gmail.com)
