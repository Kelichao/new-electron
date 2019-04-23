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

![image](https://user-images.githubusercontent.com/18028533/56497636-04cf2d00-6531-11e9-8652-2ed5b80b01c0.png)

![image](https://user-images.githubusercontent.com/18028533/56497248-5d052f80-652f-11e9-86fd-e890577bd6d6.png)

## 下载打安装包软件
[Inno Setup下载地址](https://pc.qq.com/detail/13/detail_1313.html)
- 安装参考[热心网友教程](https://www.cnblogs.com/kakayang/p/9559777.html)

![image](https://user-images.githubusercontent.com/18028533/56497449-1b28b900-6530-11e9-84fe-e92c9383f603.png)

## 打开之后，选择新建，一路确定，选择好以下两个步骤，然后一路默认确定
- 步骤一：

![image](https://user-images.githubusercontent.com/18028533/56497510-5fb45480-6530-11e9-9a67-6fb446c072b9.png)

- 步骤二：

![image](https://user-images.githubusercontent.com/18028533/56497569-ac982b00-6530-11e9-8988-f8bfca5545d4.png)

# 安装
- 打包完毕，安装即可

![image](https://user-images.githubusercontent.com/18028533/56498083-d0f50700-6532-11e9-949e-afad74c19114.png)

## electron依赖下载不下来报错的问题，切换源
1. 切换npm源，由于访问npm官方源不太稳定，因此推荐将官方源修改为国内的镜像

`npm config set registry https://registry.npm.taobao.org`

2. Electron 安装, 切换Electron Download的源

`npm config set electron_mirror="https://npm.taobao.org/mirrors/electron/"`

## getmac插件报错原因
- 之前由于getmac安装使用了`npm install getmac`导致移动目录之后，依赖丢失。
- getmac需要用`npm install getmac --save`方式，放进依赖。

# 友情赞助
[马超群友情赞助](https://note.youdao.com/ynoteshare1/index.html?id=522fe35f2a9047045200895b7383f03f&type=note)
