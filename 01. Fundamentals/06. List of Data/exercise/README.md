### 练习：使用`.map()`渲染数据列表

在本练习中，你将学习如何在JSX中使用`.map()`方法渲染项目列表。

#### 步骤1：创建`UserList`组件

1. 创建一个名为`UserList.jsx`的新文件。
2. 在该文件中，创建一个名为`UserList`的函数式组件。
3. 在组件中，创建一个包含以下对象的`users`数组，其中每个对象代表一个包含`id`、`name`和`age`的用户：

   ```javascript
   const users = [
     { id: 1, name: "Alice", age: 25 },
     { id: 2, name: "Bob", age: 30 },
     { id: 3, name: "Charlie", age: 22 },
   ];
   ```

4. 使用`.map()`方法渲染用户列表。每个用户的`name`和`age`应显示在一个`<div>`元素内。将`id`用作每个列表项的唯一`key`。

#### 步骤2：创建`ProductList`组件

1. 创建一个名为`ProductList.jsx`的新文件。
2. 在该文件中，创建一个名为`ProductList`的函数式组件。
3. 创建一个包含以下对象的`products`数组，其中每个对象代表一个包含`id`、`name`和`price`的产品：

   ```javascript
   const products = [
     { id: 1, name: "Phone", price: "$699" },
     { id: 2, name: "Laptop", price: "$1200" },
     { id: 3, name: "Headphones", price: "$199" },
   ];
   ```

4. 使用`.map()`方法渲染产品列表。每个产品的`name`和`price`应显示在一个`<div>`元素内。将`id`用作每个产品的`key`。

#### 步骤3：在`App.jsx`中渲染组件

1. 在你的`App.jsx`文件中，导入`UserList`和`ProductList`组件：

   ```jsx
   import UserList from "./UserList";
   import ProductList from "./ProductList";
   ```

2. 在`App`组件的return语句中，渲染`UserList`和`ProductList`组件：

   ```jsx
   function App() {
     return (
       <div>
         <UserList />
         <ProductList />
       </div>
     );
   }

   export default App;
   ```