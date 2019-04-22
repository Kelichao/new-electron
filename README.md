# 环境搭建
- 首先确保拥有node,npm环境
```
# 全局安装electron
$ npm install electron -g

# 安装依赖
$ npm install

# 本地调试
$ npm start 

# 生成静态打包文件（免安装版本，）
$ npm run package

```

# 打包概要
- 执行`$ npm run package`后，会生成两个文件夹，我们选取`HelloWorld-win32-x64`作为打安装包文件。
- 目录为`\outApp\HelloWorld-win32-x64`
![image](https://user-images.githubusercontent.com/18028533/56497248-5d052f80-652f-11e9-86fd-e890577bd6d6.png)
# 

## getmac插件报错原因
- 之前由于getmac安装使用了`npm install getmac`导致移动目录之后，依赖丢失。
- getmac需要用`npm install getmac --save`方式，放进依赖。
