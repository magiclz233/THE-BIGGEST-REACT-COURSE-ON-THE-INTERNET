### 练习：在React中使用`useReducer`

在本练习中，你将学习如何：

- 定义reducer函数来管理状态逻辑
- 使用`useReducer`钩子在React组件中管理复杂状态
- 分发（Dispatch）动作以更新状态

---

### 步骤1：设置Reducer函数

1. 创建一个名为`counterReducer.js`的新文件。
2. 在该文件中，定义一个reducer函数来管理简单计数器的状态。

### 步骤2：使用`useReducer`钩子

1. 创建一个名为`Counter.jsx`的新文件。
2. 在该文件中，创建一个名为`Counter`的函数式组件。
3. 使用`useReducer`钩子来管理计数器的状态。

### 步骤3：扩展Reducer以支持更多动作

1. 修改`counterReducer.js`文件，添加更多动作来实现按特定数量增加和减少计数。

### 步骤4：在动作中使用载荷（Payload）

1. 更新`Counter.jsx`文件，允许用户通过输入框按特定值增加或减少计数。

### 步骤5：在`App.jsx`中渲染计数器

1. 在你的`App.jsx`文件中，导入并渲染`Counter`组件。

```jsx
import React from "react";
import Counter from "./Counter";

function App() {
  return (
    <div>
      <h1>React useReducer示例</h1>
      <Counter />
    </div>
  );
}

export default App;
```