# React.js-Examples


* Memo

If your function component renders the same result given the same props, you can wrap it in a call to React.memo for a performance boost in some cases by memoizing the result. This means that React will skip rendering the component, and reuse the last rendered result.

Example -> https://codesandbox.io/s/react-memo-example-e0fmx

* Axios cancel request

Resolves the problem of loading relevant information after your value has changed.

If you do not cancel the previous request, the information that it claims will be random and the first one loaded will appear on the screen because it is the wrong request.

![alt text](https://i.ibb.co/7VnRyxx/Capturereq.png)

moves to detect the bug !! try to put a into input, add b to a (ab), remove b -> add bc (abc) -> remove c and put d (abd), and you get the wrong result in a screen.

you can resolve this problem with many technique like abortController, debounce-input, takeLatest in redux-saga, Observable - RxJS and cancel fetch...

Example -> https://codesandbox.io/s/cancel-previous-axios-request-vtmej
