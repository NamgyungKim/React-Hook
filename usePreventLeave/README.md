## usePreventLeave

: 페이지를 저장하지 않고 닫았을때 나타나는 경고창

```js
const App = () => {
  const { enablePrevent, disablePrevent } = usePreventLeave()
  //enablePrevent는 닫기전 경고창을 띄움
  //disablePrevent는 경고창띄우기를 해제시킴
  return (
    <div className="App">
      <button onClick={enablePrevent}>Protect</button>
      <button onClick={disablePrevent}>UnProtect</button>
    </div>
  )
}
```
