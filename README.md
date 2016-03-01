# poly-compatibility

An element providing a wrapper around Modernizr tests.


## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

The element itself requires both paper-dialog and paper-button.

## How to use

the wrapper is as thin as possible:

```
    <poly-Compatibility  path-To-Test="./modernizrtest.js" >
        sorry bud, cant help you, download one of these browsers or something!
    </poly-Compatibility>
```

the path-To-Test points to the modernizr file required for your build.
the wrapper will load the file and inspect all the booleans.
if one of them failed (is false) then the element will show a dialog informing the user!

## Things still todo:
* Add specific error message's on what property failed
