### 练习：精通React中的`useState`

在本练习中，你将学习如何在各种场景下使用`useState`钩子管理状态，包括基本用法、数组、对象以及对象数组。

#### 步骤1：`useState`的基本用法

1. 创建一个名为`Counter.jsx`的新文件。
2. 在该文件中，创建一个名为`Counter`的函数式组件。
3. 使用`useState`管理一个简单的计数器状态。
   - 将状态初始值设为`0`。
   - 创建一个按钮，点击时将计数器加`1`。
   - 显示计数器的当前值。

#### 步骤2：`useState`结合数据数组

1. 创建一个名为`TodoList.jsx`的新文件。
2. 在该文件中，创建一个名为`TodoList`的函数式组件。
3. 使用`useState`管理待办事项数组。
   - 将状态初始化为空数组。
   - 创建一个表单，用于向列表中添加新的待办事项。
   - 显示待办事项列表。

#### 步骤3：`useState`结合数据对象

1. 创建一个名为`Profile.jsx`的新文件。
2. 在该文件中，创建一个名为`Profile`的函数式组件。
3. 使用`useState`管理包含用户资料信息的对象。
   - 将状态初始化为包含`name`和`age`的对象。
   - 提供输入框用于更新`name`和`age`。
   - 显示更新后的资料信息。

#### 步骤4：`useState`结合对象数组

1. 创建一个名为`ShoppingList.jsx`的新文件。
2. 在该文件中，创建一个名为`ShoppingList`的函数式组件。
3. 使用`useState`管理对象数组，其中每个对象代表一个包含`name`和`quantity`的购物项。
   - 将状态初始化为空数组。
   - 创建一个表单，用于向列表中添加新的购物项。
   - 显示购物项列表。

#### 步骤5：在`App.jsx`中渲染所有组件

1. 在你的`App.jsx`文件中，导入`Counter`、`TodoList`、`Profile`和`ShoppingList`组件：

   ```jsx
   import Counter from "./Counter";
   import TodoList from "./TodoList";
   import Profile from "./Profile";
   import ShoppingList from "./ShoppingList";
   ```

2. 在`App`组件中，渲染这四个组件：

   ```jsx
   function App() {
     return (
       <div>
         <h1>React useState示例</h1>
         <Counter />
         <TodoList />
         <Profile />
         <ShoppingList />
       </div>
     );
   }

   export default App;
   ```