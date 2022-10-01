# DUMI 模板工程

基于 `yarn create @umijs/dumi-lib --site` 脚手架命令搭建的站点 `DUMI` 文档。 

可以直接 `git clone https://github.com/wangjs-jacky/first-dumi.git`

本模板提供：
1. 提供一个简易版本的 aHooks 模拟源码工程示例（以后将作为案例中心）

2. 使用 `babel-plugin-import` 实现按需导入 `antd` 样式文件。

     `.umirc.ts` 中添加如下代码：

     ```javascript
     {
       extraBabelPlugins: [
         [
           'import',
           {
             libraryName: 'antd',
             libraryDirectory: 'es',
             style: 'css',
           },
         ],
       ]
     }
     ```
