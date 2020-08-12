![](https://i.ibb.co/pz9HQwN/Cables.png)
<p align="center">
React examples from real world programing, solve bugs, best practice & cool stuf :)
</p>

<hr/>
 

## ⚡ React hooks Memo

When your function component renders the same result given the same props, you can wrap it in a call to React.memo for a performance boost in some cases by memoizing the result. This means that React will skip rendering the component, and reuse the last rendered result. 

[Live Example](https://codesandbox.io/s/react-memo-example-e0fmx)


## ⚡ Axios cancel request

Resolves the problem of loading relevant information after your value has changed.

If you do not cancel the previous request, the information that it claims will be random and the first one loaded will appear on the screen because it is the wrong request.

![](https://i.ibb.co/7VnRyxx/Capturereq.png)

moves to detect the bug !! try to put a into input, add b to a (ab), remove b -> add bc (abc) -> remove c and put d (abd), and you get the wrong result in a screen.

you can resolve this problem with many technique like abortController, debounce-input, takeLatest in redux-saga, Observable - RxJS and cancel fetch...

[Live Example](https://codesandbox.io/s/cancel-previous-axios-request-vtmej)

## ⚡ Retain Previous Values with React.useRef - Js Hook

Whenever we want to save the previous value a good way to do this is with the use React.useRef.
One of the reasons why it will work is because ```React.useRef``` running after Components finished rendering.
The value of ```ref.current``` will updated after render from ```useEffect```, ```ref.current``` retains the last value passed to it in a previous renderer.

[Live Example](https://codesandbox.io/s/retain-previous-values-js-hook-mkc0v)

## ⚡ Search get value from json data in background using web worker

> A worker is an object created using a constructor (e.g. Worker()) that runs a named JavaScript file — this file contains the code that will run in the worker thread; workers run in another global context that is different from the current window. [source](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API)

[React-Web-Worker](https://github.com/davidkern13/react-web-worker)

## ⚡ Use react custom middleware for axios call to post,put,delete,update

Instead of creating a file of server requests, you can create one custom Middleware file and pass through the action that you want to perform on a server call.

[React-Middleware-Axios](https://github.com/davidkern13/react-middleware-axios)

## ⚡ React rxjs observable example how to get updated data from server. 

There is a possibility that the server first returns irrelevant information and then updates the information to json list, because we do not know when the information will be updated we need to listen to the changes.

Peterson Observer is great solution for this problem, can be exercised with rxjs or custom js.

[React-rxjs-observable](https://github.com/davidkern13/react-rxjs-observable)

## ⚡ Implementation custom socket middleware with react hooks & redux

 Web socket custom middleware for get real time data from server.

[React-Hooks-Socket-Middleware](https://github.com/davidkern13/react-hooks-socket-middleware)

## ⚡ Use React-Lazy-Image when you have image in your ui

#### Check the codesandbox [example](https://codesandbox.io/s/zen-dijkstra-jh20d?file=/src/App.js), copy the code to your project and follow next steps to get result.

[React-Lazy-Image](https://github.com/davidkern13/React-Lazy-Image)

## ⚡ JavaScript Features in ES2020

#### New javascript features.

[JavaScript-Features-in-ES2020](https://github.com/davidkern13/JavaScript-Features-in-ES2020)


## ⚡ React hook useReducer example

#### check the sample.

[React hook useReducer example](https://codesandbox.io/s/react-hook-usereducer-example-8952b)

## ⚡ React hook useInputValue example

#### useInputValue custom hook to help us to make the component more cleaner, readable and efficiently.

[React hook useInputValue example](https://codesandbox.io/s/useinputvalue-43k9d?file=/src/App.js:0-1071)

## ⚡ React hook useAuth example

#### useAuth custom hook to help us to make the component more cleaner, readable and efficiently.

[React hook useInputValue example](https://codesandbox.io/s/react-hooks-useauth-duc9w)





