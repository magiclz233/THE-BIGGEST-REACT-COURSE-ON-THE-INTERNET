### 练习：在JSX中使用`{}`实现动态内容

在本练习中，你将学习如何使用花括号`{}`向JSX中注入动态数据。

#### 步骤1：创建`Greeting`组件

1. 创建一个名为`Greeting.jsx`的新文件。
2. 在该文件中，创建一个名为`Greeting`的函数式组件。
3. `Greeting`组件应返回一个包含以下内容的`<div>`：

   - 一个`<h1>`元素，用于动态显示问候语。
   - 一个`<p>`元素，用于动态显示当前日期。

4. 在`{}`内使用JavaScript表达式来动态渲染以下内容：
   - 一个包含姓名的`name`变量，例如`"John"`。
   - 一个`new Date()`对象，用于显示当前日期。

#### 步骤2：创建`ProductInfo`组件

1. 创建一个名为`ProductInfo.jsx`的新文件。
2. 在该文件中，创建一个名为`ProductInfo`的函数式组件。
3. `ProductInfo`组件应返回一个`<div>`，用于动态显示产品详情：

   - 使用一个包含以下属性的`product`对象：
     - `name`：`"Laptop"`，
     - `price`：`$1200`，
     - `availability`：`"In stock"`（有货）

4. 使用`{}`显示产品名称、价格和库存状态。

#### 步骤3：在`App.jsx`中渲染组件

1. 在你的`App.jsx`文件中，导入`Greeting`和`ProductInfo`组件：

   ```jsx
   import Greeting from "./Greeting";
   import ProductInfo from "./ProductInfo";
   ```

2. 在`App`组件的return语句中，渲染这两个组件：

   ```jsx
   function App() {
     return (
       <div>
         <Greeting />
         <ProductInfo />
       </div>
     );
   }

   export default App;
   ```