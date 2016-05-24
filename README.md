# VueJs Boilerplate - Babel / Webpack / Sass

![Banner](http://i.imgur.com/kJepFbl.png)


#### TECHNOLOGIES

* VueJs
* EventEmitter
* GSAP - TweenMax
* Babel | ES2015
* Webpack
* ESLint
* SASS


##### EventManagerMixin

EventManagerMixin handle Emitter events and DOM events easily. It will auto bind the context, and dettach the event when the component will unmount.

If you want to use the EventManager mixin, you need to define emitterEvents / domEvents in your vue component like so :

```
export default Vue.extend({

  mixins: [EventManagerMixin],

  emitterEvents: [{
    message: WINDOW_RESIZE, // Event Message
    method: 'onWindowResize' // Name of the method
    once: false, // Optional - Listen to the event once or not, default: false
  }],

  domEvents: [{
    target: document, // DOM element to attach the event
    event: 'mousemove', // Event type
    method: 'handleDocumentMouseMove' // Name of the method
  }],

...
}
```


##### Install dependancies :
```shell
  npm i
```


##### Launch the project :
```shell
  npm start
```


The project will be launched at http://localhost:3000/


##### Build for production :
```shell
  npm run build
```

#### CONTRIBUTORS
* [Fabien Motte](http://example.com "Fabien Motte")
* [Patrick Heng](http://example.com "Patrick Heng")



Hope you like it ¯\_(ツ)_/¯

![Gif](https://media.giphy.com/media/yGEbmgiCJYu3u/giphy.gif)
