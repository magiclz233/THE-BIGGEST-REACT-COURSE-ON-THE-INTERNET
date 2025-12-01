### 练习：在React中使用Context和`useContext`

在本练习中，你将学习如何：

- 创建Context
- 使用`useContext`从Context中访问数据
- 在组件之间共享状态和函数，无需使用props

#### 步骤1：创建Context

1. 创建一个名为`UserContext.js`的新文件。
2. 在该文件中，创建一个`UserContext`和一个`UserProvider`组件，用于存储共享状态。

#### 步骤2：在组件中使用`useContext`

1. 创建一个名为`UserProfile.jsx`的新文件。
2. 在该文件中，创建一个名为`UserProfile`的函数式组件。该组件将使用`useContext`钩子从`UserContext`中访问用户数据。

#### 步骤3：更新Context数据

1. 创建一个名为`UpdateUser.jsx`的新文件。
2. 在该文件中，创建一个名为`UpdateUser`的函数式组件，允许用户更新他们的姓名。