> 组件开发有很多中方式，比如使用React/Vue或者使用符合AMD规范的库；其实mendix官网开发的组件是使用的dojo开发。

> 如果有同学没有学习过Vue/React开发，但是对原生Javascript有一定了解的话，请移步[开发一个简单组件需要的步骤](http://note.youdao.com/noteshare?id=b2eb116aa4bc96e6f82a0ce10cbe1c1e)和[组件开发引入外部符合AMD规范的库存在的问题](http://note.youdao.com/noteshare?id=06403f0b04a179cbe1d4864ae2145bd4)。我想在以上可以找到答案。

> 本文不详细解释如何使用Vue开发一个页面，如果您有使用Vue开发Mendix组件的需求，
那么请直接点击下载[Mendix组件开发之Vue基础包](https://github.com/MrGaoGang/mendix_vue_template.git)。
使用基础包开发会减少您的开发周期，如果基础包有什么问题请联系我gaogangwork@qq.com。



# 使用Vue开发Mendix组件模板 
[English](./README.md)

如果你对mendix组件开发基础知识还不了解的话，请先移步[个人博客-mendix组件开发专题](https://mrgaogang.github.io/article/mendix/widgets/%E8%AF%A6%E7%BB%86API.html)

> 由于mendix只在Windows中有客户端，所以必须在windows中国使用此模板。

使用步骤如下：
### 1. 安装git和zip

第一步: 建议你使用git命令行来构建组件。git下载地址是 [点击这里下载](https://git-scm.com/downloads);
第二步: 安装 **zip and bzip2** [点击去这里下载zip和bzip2](https://sourceforge.net/projects/gnuwin32/files/)

我下载的是“zip-3.0-bin.zip” 和 “zip.exe” ， “bzip2-1.0.5-bin.zip” 和 “bzip2.dll” /bin/.exe
记住：**将zip.exe文件和bzip2.dll文件拷贝到git安装目录下**




### 2. 如何使用
第一步: 下载这个模板或者 git clone https://github.com/MrGaoGang/mendix_vue_template
第二步: 打开组件开发根目录
第三步:运行如下命令

```bash
npm install
npm run build
```
如果你想打生产包的组件的话，请修改webpack.config.js的文件
```js
   mode: "development", // Change the mode do "production" before you go live! Don't forget!
    plugins: [
        // Change the plugin do "production" before you go live! Don't forget!
        new webpack.DefinePlugin({
            'process.env': {
                NODE_ENV: '"development"' // change to "production" when publishing your Mendix widget
            }
        }),

```




### 致谢

十分感谢 https://intonovi.com 封装了基础模板，其Github地址为[here](https://github.com/Intonovi/mendix-vuejs-widget-boilerplate)；本项目是基于此模板进行的优化和改良。



