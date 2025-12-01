### 练习：在React组件中使用Props

在本练习中，你将学习如何在React组件中传递和使用props，使组件具有动态性和可复用性。

#### 步骤1：创建`Person`组件

1. 创建一个名为`Person.jsx`的新文件。
2. 在该文件中，创建一个名为`Person`的函数式组件。
3. 该组件应接收`props`并渲染：

   - 一个`<h2>`元素，显示人物的姓名。
   - 一个`<p>`元素，显示人物的年龄。

4. 使用`props.name`和`props.age`来显示从父组件传递过来的动态值。

#### 步骤2：创建`Product`组件

1. 创建一个名为`Product.jsx`的新文件。
2. 在该文件中，创建一个名为`Product`的函数式组件。
3. 该组件应接收`props`并渲染：

   - 一个`<h2>`元素，显示产品的名称。
   - 一个`<p>`元素，显示产品的价格。

4. 使用`props.name`和`props.price`来显示从父组件传递过来的值。

#### 步骤3：从`App.jsx`传递Props

1. 在你的`App.jsx`文件中，导入`Person`和`Product`组件：

   ```jsx
   import Person from "./Person";
   import Product from "./Product";
   ```

2. 在`App`组件内部，将动态数据作为props传递给`Person`和`Product`组件：
   - 向`Person`组件传递`name`和`age`作为props。
   - 向`Product`组件传递`name`和`price`作为props。