# ⚠️ 学习"useState"钩子时完成此练习 ⚠️

### 挑战：在React中处理事件

#### 步骤1：创建`EventDemo`组件

1. 创建一个名为`EventDemo.jsx`的新文件。
2. 在该文件中，创建一个名为`EventDemo`的函数式组件。
3. 该组件应渲染以下元素：

   - 一个`<button>`按钮，点击时将`<p>`元素的文本更新为"Button Clicked!"（按钮已点击！）。
   - 一个包含`<p>`元素的`<div>`。当`<p>`元素内的文本被复制时，文本应改为"Text Copied!"（文本已复制！）。
   - 一个包含`<p>`元素的`<div>`。当鼠标悬停在`<p>`元素上时，背景颜色应变为浅黄色。

#### 步骤2：在`App.jsx`中渲染`EventDemo`组件

1. 在你的`App.jsx`文件中，导入`EventDemo`组件：

   ```jsx
   import EventDemo from "./EventDemo";
   ```

2. 在`App`组件中，渲染`EventDemo`组件：

   ```jsx
   function App() {
     return (
       <div>
         <h1>React事件处理挑战</h1>
         <EventDemo />
       </div>
     );
   }

   export default App;
   ```