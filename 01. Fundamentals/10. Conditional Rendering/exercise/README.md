### 练习：React中的条件渲染

在本练习中，你将练习在React组件中以不同方式进行JSX的条件渲染。

#### 步骤1：使用`if`、`else if`和`else`创建`Weather`组件

1. 创建一个名为`Weather.jsx`的新文件。
2. 在该文件中，创建一个名为`Weather`的函数式组件。
3. 该组件应：
   - 接收一个`temperature`属性（prop）。
   - 使用`if`、`else if`和`else`语句根据温度值有条件地渲染不同的消息：
     - 如果温度低于15，显示："外面很冷！"
     - 如果温度在15到25之间，显示："外面天气很好！"
     - 如果温度高于25，显示："外面很热！"

#### 步骤2：使用`&&`运算符创建`UserStatus`组件

1. 创建一个名为`UserStatus.jsx`的新文件。
2. 在该文件中，创建一个名为`UserStatus`的函数式组件。
3. 该组件应：
   - 接收两个布尔类型的属性（prop）：`loggedIn`和`isAdmin`
   - 使用`&&`运算符为管理员和普通用户显示不同的消息：
     - 如果`loggedIn`为`true`且`isAdmin`为真，显示："欢迎管理员！"
     - 如果仅`loggedIn`为真且不是管理员，则显示"欢迎用户"。

#### 步骤3：使用三元运算符创建`Greeting`组件

1. 创建一个名为`Greeting.jsx`的新文件。
2. 在该文件中，创建一个名为`Greeting`的函数式组件。
3. 该组件应：
   - 接收一个`timeOfDay`属性（prop）（例如：`"morning"`、`"afternoon"`或`"evening"`）。
   - 使用三元运算符根据一天中的不同时段有条件地显示不同的问候语：
     - 如果`timeOfDay`是`"morning"`，显示："早上好！"
     - 如果`timeOfDay`是`"afternoon"`，显示："下午好！"

#### 步骤4：在`App.jsx`中渲染组件

1. 在你的`App.jsx`文件中，导入`Weather`、`UserStatus`和`Greeting`组件：

   ```jsx
   import Weather from "./Weather";
   import UserStatus from "./UserStatus";
   import Greeting from "./Greeting";
   ```

2. 在`App`组件内部，传递不同的属性（prop）渲染每个组件，以测试条件渲染逻辑。

示例：

```jsx
function App() {
  return (
    <div>
      <h1>React中的条件渲染</h1>

      {/* Weather组件 */}
      <Weather temperature={10} />
      <Weather temperature={20} />
      <Weather temperature={30} />

      {/* UserStatus组件 */}
      <UserStatus loggedIn={true} isAdmin={true} />
      <UserStatus loggedIn={true} isAdmin={false} />
      <UserStatus loggedIn={false} />

      {/* Greeting组件 */}
      <Greeting timeOfDay="morning" />
      <Greeting timeOfDay="afternoon" />
      <Greeting timeOfDay="evening" />
    </div>
  );
}

export default App;
```