## useConfirm

: 사용자에게 실행전 실행여부 재확인

```js
const App = () => {
  const deleteWorld = () => console.log('Deleting the world')
  const abort = () => console.log('Aborted')
  const confirmDelete = useConfirm('Are you sure?', deleteWorld, abort)
  //useConfirm(alart문자, 확인클릭시 실행시킬 함수, 취소 클릭시 실행시킬 함수)
  return (
    <div className="App">
      <button onClick={confirmDelete}>Delete the world</button>
    </div>
  )
}
```
