## useTitle

: title업데이트

```js
const App = () => {
  const titleUpdater = useTitle('Lodding...')
  setTimeout(() => titleUpdater('Home'), 5000)
  return (
    <div className="App">
      <div>Hi</div>
    </div>
  )
}
```
