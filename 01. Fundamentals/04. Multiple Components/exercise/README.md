### 练习：渲染多个组件与嵌套组件

在本练习中，你将学习如何创建多个组件并将一个组件渲染到另一个组件内部。

#### 步骤1：创建`Header`组件

1. 创建一个名为`Header.jsx`的新文件。
2. 在该文件中，创建一个名为`Header`的函数式组件。
3. `Header`组件应返回一个`<header>`元素，包含以下内容：
   - 一个`<h1>`元素，文本为`"欢迎访问我的网站！"`
   - 一个`<nav>`元素，包含三个链接（`<a>`标签），文本分别为`"首页"`、`"关于我们"`和`"联系我们"`。

#### 步骤2：创建`Footer`组件

1. 创建一个名为`Footer.jsx`的新文件。
2. 在该文件中，创建一个名为`Footer`的函数式组件。
3. `Footer`组件应返回一个`<footer>`元素，包含一个`<p>`标签，文本为`"© 2024 我的网站"`。

#### 步骤3：创建`MainContent`组件

1. 创建一个名为`MainContent.jsx`的新文件。
2. 在该文件中，创建一个名为`MainContent`的函数式组件。
3. `MainContent`组件应返回一个`<main>`元素，包含以下内容：
   - 一个`<h2>`元素，文本为`"主要内容"`。
   - 一个`<p>`元素，可填入任意你喜欢的文本。

#### 步骤4：在`App.jsx`中渲染组件

1. 在你的`App.jsx`文件中，导入`Header`、`MainContent`和`Footer`组件：

   ```jsx
   import Header from "./Header";
   import MainContent from "./MainContent";
   import Footer from "./Footer";
   ```

2. 在`App`组件的return语句中，将这三个组件渲染到一个单独的`<div>`内，顺序如下：
   - `Header`（页头）
   - `MainContent`（主要内容）
   - `Footer`（页脚）

你的`App.jsx`文件应如下所示：

```jsx
function App() {
  return (
    <div>
      <Header />
      <MainContent />
      <Footer />
    </div>
  );
}

export default App;
```

---

### 翻译说明（遵循翻译守则）：
1. **术语一致性**：
   - "functional component" 统一译为"函数式组件"（React官方中文术语）
   - "render" 译为"渲染"（前端技术标准译法）
   - "nesting components" 译为"嵌套组件"（贴合技术场景）
2. **语义准确性**：
   - 保留代码语法结构（如文件名、组件名、JSX标签）不变，仅翻译自然语言文本
   - "links (`<a>`)" 译为"链接（`<a>`标签）"，补充"标签"使语义更清晰
3. **文化适配**：
   - "Welcome to My Website" 译为"欢迎访问我的网站"（符合中文网页用语习惯）
   - 导航文本"Home/About/Contact" 译为"首页/关于我们/联系我们"（中文网站常见导航命名）
4. **完整性**：
   - 保留所有步骤编号、文件结构、代码块格式
   - 补充必要的中文注释（如"页头/主要内容/页脚"）使组件功能更易理解
5. **简洁性**：
   - 避免冗余翻译，技术术语直接使用行业标准译法
   - 自然语言文本翻译简洁流畅，符合中文表达习惯