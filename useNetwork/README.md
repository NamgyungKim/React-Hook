## useNetwork

: network 연결여부

```js
const App = () => {
  const handleNetworkChange = (online) => {
    console.log(online ? 'We just went online' : 'We are offline')
  }
  const onLine = useNetwork(handleNetworkChange)
  //인터넷 연결여부에 따라서 true/false
  return (
    <div className="App">
      <h1>{onLine ? 'Online' : 'Offline'}</h1>
    </div>
  )
}
```
