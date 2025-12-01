### 练习：React中的组件样式设置

在本练习中，你将学习如何在React组件中使用不同方法应用样式，包括内联样式、样式对象以及React图标。

#### 步骤1：使用内联样式创建`StyledCard`组件

1. 创建一个名为`StyledCard.jsx`的新文件。
2. 在该文件中，创建一个名为`StyledCard`的函数式组件。
3. 使用内联样式为组件设置样式：

   - 将背景颜色设置为浅蓝色。
   - 将内边距设置为`20px`。
   - 将边框圆角设置为`10px`。
   - 将文本颜色设置为深蓝色。

4. 渲染一个包含标题和描述的`<div>`。

#### 步骤2：使用独立样式对象创建`ProfileCard`组件

1. 创建一个名为`ProfileCard.jsx`的新文件。
2. 在该文件中，创建一个名为`ProfileCard`的函数式组件。
3. 定义一个`styles`对象来存放CSS属性：

   - 将背景颜色设置为浅灰色。
   - 将内边距设置为`15px`。
   - 将边框圆角设置为`8px`。
   - 将文本颜色设置为黑色。

4. 使用`style`属性将`styles`对象应用到`<div>`上。

5. 渲染一个包含标题和描述的`<div>`。

#### 步骤3：使用React图标创建`IconComponent`

1. 如果尚未安装`react-icons`，请执行安装：

   ```bash
   npm install react-icons
   ```

2. 创建一个名为`IconComponent.jsx`的新文件。
3. 在该文件中，创建一个名为`IconComponent`的函数式组件。
4. 从`react-icons`中导入一个图标，例如从`react-icons/fa`中导入`FaBeer`。

5. 使用内联样式为图标设置样式：

   - 将字体大小设置为`30px`。
   - 将颜色设置为金色。

6. 渲染带有标题的图标。

#### 步骤4：在`App.jsx`中渲染所有组件

1. 在你的`App.jsx`文件中，导入`StyledCard`、`ProfileCard`和`IconComponent`组件：

   ```jsx
   import StyledCard from "./StyledCard";
   import ProfileCard from "./ProfileCard";
   import IconComponent from "./IconComponent";
   ```

2. 在`App`组件中，渲染这三个组件：

   ```jsx
   function App() {
     return (
       <div>
         <StyledCard />
         <ProfileCard />
         <IconComponent />
       </div>
     );
   }

   export default App;
   ```