---
title: React Javascript Framework
tags:
- react
- javascript
- framework
---

# React Javascript Framework

<TagLinks />

## React

* javascript library
* maintained by facebook
* Additional libraries
  * Redux - state management
  * React router
* React Hooks
* React native to build native mobile apps
* [MV-VC Model](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93viewmodel)
* [CRA - Creatre react app](https://create-react-app.dev/docs/getting-started)
  * less to learn about react build toolchains
* [How to solve npm, node and dotnetcore version problem? Use yarn with dotnet](https://stackoverflow.com/questions/60794367/asp-net-core-3-1-integration-with-npm)
* Is it a js framework? or a js library?
* Components have its own states

> In React components, code reuse is primarily achieved through composition rather than inheritance.

How to implement state into component?
:   There are 2 ways

    1. `class` component
    2. Use new `hooks`


## How to learn

* javascript ES6 (Objects, Arrays, Conditionals, Classes, types, async await, Promises, arrow fn, destructuring)
* Components have states
* states can be updated on certain browser events
* Anatomy of a Component
  * component extends to `React.Component` Class
  * `render()` lifecycle method returns `JSX`
* [React developer tools](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi/related?hl=en)
* create-react-app is like a CLI
* react-scripts - webpack magic
  * eject - if you want to customize webpack files
* How data and props are added to components?
  * each componet have state Object
  * this.props.todos.map((todo) => (<h3>{ todo.title }</h3>))

[Is there a limit on # files git can track?](https://stackoverflow.com/questions/984707/what-are-the-file-limits-in-git-number-and-size)

###### How HTTP works?


[Why need a 3-way handshake? Why is not 2-way handshake enough?](https://networkengineering.stackexchange.com/questions/24068/why-do-we-need-a-3-way-handshake-why-not-just-2-way?newreg=78238e3261a247cfb7bebeeee54f4f2d)

![HTTP 3-way Handshake sequence diagram](https://miro.medium.com/max/2612/1*n22QJMww4vGw_MrlZbysLg.png)

![OSI reference model data units](https://banner2.cleanpng.com/20181113/qbx/kisspng-osi-model-transport-layer-data-link-layer-computer-5beaba79d22172.8903284315421098178607.jpg)

## How website works

1. Browser (cilent) makes a request to server (website server), like google.com etc
2. Server respods to client request and starts transmitting response
3. response is downloaded by Browser
4. Browser parses the response
5. Browser generates a DOM - DOMContentLoaded
6. browser issues document.Load event
7. control is passed to react js
8. react js maintains a virtual-DOM. Why?
   1. apparently writes/frequent modifications to traditional DOM are expensive
   2. so we minimize write to DOM my maintaining a virtual DOM
   3. How virtual DOM is synced with actual DOM? Reconcilation step
   4. by taking diff and updating only the parts/elements which needs to update and leave the remaining tree un touched
      1. better than recreating entire DOM on every update

![virtual DOM reconcilation](https://res.infoq.com/presentations/react-reconciliation/en/slides/sl23.jpg)
![virtual DOM diff computation](https://blog.codecentric.de/files/2017/11/Bildschirmfoto-2017-10-25-um-14.32.03.png)

virtual DOM
: in-memory datastructure cache

```js{2,3}
ReactDOM.render(
  <h1>Hello, world!</h1>,             // element
  document.getElementById('root')     // container
);
```

## Dotnet react app

```js
node --version
v10.19.0
npm --version
6.14.4
dotnet --version
3.1.202
tsc --version
Version 3.9.2

```

### Debugging

* vscode
* Debugger for Chrome - talk to google devtools protocol API
*







*[JSX]: Javascript and XML

<Footer />
