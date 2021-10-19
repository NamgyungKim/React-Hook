## useTabs

: Tab 버튼

```js
// tab이름과 content내용
const content = [
  {
    tab: 'Section 1',
    content: "I'm the content of the Section 1",
  },
  {
    tab: 'Section 2',
    content: "I'm the content of the Section 2",
  },
  {
    tab: 'Section 3',
    content: "I'm the content of the Section 3",
  },
]

const App = () => {
  const { currentItem, changeItem } = useTabs(0, content)
  // useTabs(초기값 배열0번부터 보영줌, 배열이름)
  return (
    <div className="App">
      {content.map((section, index) => (
        <button onClick={() => changeItem(index)}>{section.tab}</button>
      ))}
      <div>{currentItem.content}</div>
    </div>
  )
}
```
