### 练习：理解React中的`useEffect`

在本练习中，你将在不同场景下练习使用`useEffect`钩子，包括获取数据、处理副作用等。

#### 步骤1：`useEffect`的基本用法

1. 创建一个名为`BasicEffect.jsx`的新文件。
2. 在该文件中，创建一个名为`BasicEffect`的函数式组件。
3. 使用`useEffect`在组件挂载时（即首次渲染时）向控制台打印一条消息。

#### 步骤2：带依赖项的`useEffect`

1. 创建一个名为`CounterEffect.jsx`的新文件。
2. 在该文件中，创建一个名为`CounterEffect`的函数式组件。
3. 使用`useEffect`在计数器值变化时更新文档标题。
   - 使用`useState`初始化`count`状态为`0`。
   - 渲染一个用于增加计数的按钮。
   - 使用`useEffect`在`count`变化时更新文档标题。

#### 步骤3：使用`useEffect`获取数据

1. 创建一个名为`FetchDataEffect.jsx`的新文件。
2. 在该文件中，创建一个名为`FetchDataEffect`的函数式组件。
3. 使用`useEffect`在组件挂载时从API获取数据。
   - 使用API端点`https://jsonplaceholder.typicode.com/posts`获取一些数据。
   - 将数据存储在状态变量中，并显示第一篇帖子的标题。