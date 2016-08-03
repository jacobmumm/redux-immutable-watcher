# Redux-Immutable-Watcher

### Install

```sh
npm install redux-immutable-watcher
```

### How It Works

redux-immutable-watcher provides a mechanism for specifying watchers that will observe the redux store. Unlike similar projects where you watch a path + key combination, this library requires that you provide a selector function. This can be any function, but would most likely be a reselect selector. 

```sh
name - any key
selector - a function which returns a value from the redux store
comparator - (optional) method of comparing two values for equality (previous and current)
cb - a callback function to invoke when the selector result has changed

watch (name, selector, comparator, cb) {}

unwatch(name) {}

```

