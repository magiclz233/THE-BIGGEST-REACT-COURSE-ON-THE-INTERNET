### 练习：React组件中的Props解构

在本练习中，你将学习如何使用**解构**来简化在React组件中访问props的方式。

#### 步骤1：创建带Props解构的`Person`组件

1. 创建一个名为`Person.jsx`的新文件。
2. 在该文件中，创建一个名为`Person`的函数式组件。
3. 直接在函数参数中解构`name`和`age` props，并渲染：
   - 一个`<h2>`元素，显示人物的姓名。
   - 一个`<p>`元素，显示人物的年龄。

#### 步骤2：创建带Props解构的`Product`组件

1. 创建一个名为`Product.jsx`的新文件。
2. 在该文件中，创建一个名为`Product`的函数式组件。
3. 在函数参数中解构`name`和`price` props，并渲染：
   - 一个`<h2>`元素，显示产品的名称。
   - 一个`<p>`元素，显示产品的价格。

#### 步骤3：从`App.jsx`传递Props

1. 在你的`App.jsx`文件中，导入`Person`和`Product`组件：

   ```jsx
   import Person from "./Person";
   import Product from "./Product";
   ```

2. 在`App`组件内部，向`Person`组件传递`name`和`age` props，向`Product`组件传递`name`和`price` props。

示例：

```jsx
function App() {
  return (
    <div>
      {/* 向Person传递props */}
      <Person name="John Doe" age={28} />
      <Person name="Jane Smith" age={32} />

      {/* 向Product传递props */}
      <Product name="Laptop" price="$1200" />
      <Product name="Smartphone" price="$699" />
    </div>
  );
}

export default App;
```