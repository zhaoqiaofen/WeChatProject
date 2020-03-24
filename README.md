# WeUI in WePY

[WeUI](https://github.com/weui/weui-wxss) 是一套同微信原生视觉体验一致的基础样式库，由微信官方设计团队为微信内网页和微信小程序量身设计，令用户的使用感知更加统一。
这里是 WeUI 在 WePY 中的使用示例。

## 体验步骤

#全局安装或更新WePY命令行工具

npm install wepy-cli -g

#在开发目录中生成Demo开发项目, 1.7.0之后版本请移步wepy-cli文档

wepy new myproject
1.7.0之后的版本使用 wepy init standard myproject 初始化项目，使用 wepy list 查看项目模板

###切换至项目目录

cd myproject

###安装依赖

npm  install

###开启实时编译

wepy build --watch or wepy build or npm run dev

### 5.导入至开发者工具

编译完成后会生成`dist`目录，开发者工具本地开发目录指向`dist`目录。

**切记： 取消勾选`项目-->开启ES6转ES5`，否则代码运行报错。**

##如果在微信开发者工具进行真机调试的时候提示源码包超出最大限制，则将本地图片上传至云端，再`删除dist文件`，重新编译即可