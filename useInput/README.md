## 사용법

: input 의 value 데이터 바인딩과 value 유효성검사 기능

```js
// index.js
const App = () => {
  const maxLen = (value) => value.includes('@')

  const name = useInput('namgyung', maxLen)

  return (
    <div className="App">
      <h1>Hello</h1>
      <input placeholder="Name" {...name} />
    </div>
  )
}
```
