# things-ws

## This is a screen for subscribing websocket information through things-ws-subscriber.

```html
    <things-ws-subscriber id="subscriber"
                          !auto
                          url-key="wsUrl"
                          subject="'/elidom/stomp/topic/hatiolab-hq/smart/'[[data.name]]">
    </things-ws-subscriber>
```

The following event is fired.

```js
        this.fire('iron-signal',{name:'subscribed', data: message})
```


*****
</br></br>

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polymer-cli

And you can run it via:

    polymer serve

Once running, you can preview your element at
`http://localhost:8080/components/things-ws/`, where `things-ws` is the name of the directory containing it.
