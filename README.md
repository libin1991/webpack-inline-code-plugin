# webpack内联代码插件
将一些常用的js css文件内联到index.html中

### 用法：
传一个数组，第一个表示要内联的js路径列表，第二个是css路径列表
css插入<head>标签中，js插入<body>标签中
按数组顺序插入

安装：
`cnpm install webpack-inline-code-plugin -D`
  

webpack.config.js配置：
```
const WebpackInlineSourcePlugin = require('webpack-inline-code-plugin');


new WebpackInlineSourcePlugin([{
	path:['./xx/xx/xx.js','./xx/xx/xx.js']
},{
	path:['./xx/xx/xx.css']
}]),
```
