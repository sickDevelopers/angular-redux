# Angular Redux
###### Angular bindings for [Redux](https://github.com/sickDevelopers/angular-redux).

*Use Redux pattern in your Angular application today. No ES6 / Js2015.*

*If you need a more complete version and you don't mind using a transpiler, use [ngAngular](https://github.com/wbuchwalter/ng-redux)*


## Table of Contents

- [Installation](#installation)
- [Quick Start](#quick-start)
- [API](#api)


## Installation
#### npm
```js
// NO NPM PACKAGE AVAILABLE
```
#### bower
```js
bower install --save angular-redux
```

Add the following script tag to your html:

```html
<script src="bower_components/angular-redux/redux.js"></script>
```

## Quick Start

#### Initialization

```JS
angular.module('app', [
	'Redux'
	])
	.config([ReduxProvider,  function(ReduxProvider) {
	    ReduxProvider.createStore(reducer, initialState);
	  }])
;
```

#### Usage

```JS
// see index.html
```

### Store API
All of redux's store methods (i.e. `dispatch`, `subscribe` and `getState`) are exposed by Redux and can be accessed directly. For example:

```JS
Redux.subscribe(function() {
    var state = Redux.getState();
});
```
