# Magitek Clicker

A simple clicker style game set in a Magitek world.

## Inspiration

* [Cookie Clicker](http://orteil.dashnet.org/cookieclicker/)
* [Final Fantasy Magitek Armor](http://finalfantasy.wikia.com/wiki/Magitek_Armor)

## Details
* [re-frame](https://github.com/Day8/re-frame) for excellent application framework
* [soda-ash](https://github.com/gadfly361/soda-ash) to wrap semantic-ui-react
* [semantic-ui-react](https://react.semantic-ui.com/introduction) for great react components

## Development Mode

### Start Cider from Emacs:

Put this in your Emacs config file:

```
(setq cider-cljs-lein-repl "(do (start) (cljs-repl))")
```

Navigate to a clojurescript file and start a figwheel REPL with `cider-jack-in-clojurescript` or (`C-c M-J`)

### Compile css:

Compile css file once.

```
lein less once
```

Automatically recompile css file on change.

```
lein less auto
```

### Run application:

```
lein clean
lein figwheel dev
```

Figwheel will automatically push cljs changes to the browser.

Wait a bit, then browse to [http://localhost:3449](http://localhost:3449).

## Production Build


To compile clojurescript to javascript:

```
lein clean
lein cljsbuild once min
```
