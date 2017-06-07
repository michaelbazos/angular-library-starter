# ui-toolkit

A library of UI components for your Angular 2 application.

Compliant with the [Angular Package Format v4.0](https://goo.gl/AMOU5G).

## Getting started

1. Install the library

  With npm: 
  ```
  npm install ui-toolkit --save   // --save is implicit as of npm 5.0
  ```

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
