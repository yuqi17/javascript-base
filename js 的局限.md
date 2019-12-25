js 目前的单线程模式，在前端注定是没法做出流畅的，复杂的动画或者说游戏。it's pity!!!!

例如 react 如果想用在动画结束的事件回调中处理state 是不允许的：
```javascript
index.js:1 Warning: Cannot update during an existing state transition (such as within `render`). Render methods should be a pure function of props and state.
```
