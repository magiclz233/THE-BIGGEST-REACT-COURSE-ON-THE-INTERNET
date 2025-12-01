### 练习：在React中创建和使用自定义钩子

在本练习中，你将学习如何：

- 创建封装状态和逻辑的自定义钩子。
- 在多个组件中复用自定义钩子。
- 创建用于处理表单输入和从API获取数据的钩子。

---

### 步骤1：创建用于切换布尔状态的自定义钩子

1. 创建一个名为`useToggle.js`的新文件。
2. 在该文件中，定义一个名为`useToggle`的自定义钩子，用于在`true`和`false`之间切换布尔值。

### 步骤2：在组件中使用自定义钩子

1. 创建一个名为`ToggleComponent.jsx`的新文件。
2. 在该文件中，创建一个组件，使用`useToggle`钩子来切换消息的显示状态。

### 步骤3：创建用于管理表单输入的自定义钩子

1. 创建一个名为`useInput.js`的新文件。
2. 在该文件中，定义一个名为`useInput`的自定义钩子，用于处理表单输入的变化。

### 步骤4：在表单组件中使用`useInput`钩子

1. 创建一个名为`FormComponent.jsx`的新文件。
2. 在该文件中，创建一个表单组件，使用`useInput`钩子来管理多个输入字段。

### 步骤5：创建用于从API获取数据的自定义钩子

1. 创建一个名为`useFetch.js`的新文件。
2. 在该文件中，定义一个名为`useFetch`的自定义钩子，用于从API获取数据，并返回数据、加载状态以及可能的错误。

### 步骤6：在组件中使用`useFetch`钩子获取数据

1. 创建一个名为`FetchComponent.jsx`的新文件。
2. 在该文件中，创建一个组件，使用`useFetch`钩子来显示从API获取的数据。

### 步骤7：在`App.jsx`中渲染所有组件

1. 在你的`App.jsx`文件中，导入并渲染`ToggleComponent`、`FormComponent`和`FetchComponent`组件。

```jsx
import React from "react";
import ToggleComponent from "./ToggleComponent";
import FormComponent from "./FormComponent";
import FetchComponent from "./FetchComponent";

function App() {
  return (
    <div>
      <h1>React自定义钩子示例</h1>
      <ToggleComponent />
      <FormComponent />
      <FetchComponent />
    </div>
  );
}

export default App;
```

---