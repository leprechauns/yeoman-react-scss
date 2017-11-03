# yeoman-react-scss
some problem solution for creating an react project
***
## 使用yeoman 快速创建一个react项目
#### 安装 yeoman
>$  npm install -g yo
#### 安装 generator-react-webapck
>$  npm install -g generator-react-webpack
#### 新建一个工程 cd 到工程目录
>根据提示创建项目
#### 启动开发环境服务器
>$  npm start
//或者</br>
$  npm run serve
#### 启动压缩版本的服务器
>$  npm run serve:dist</br>
//</br>
$  npm run dist</br>
可以使dist下文件显示；
#### 测试
>$  npm test
#### 安装可以兼容各种浏览器的css依赖
>$ cnpm autoprefixer-loader --save-dev</br>
$ cnpm sass-loader --save-dev 新版本webpack需要安装</br>
$ cnpm json-loader --save-dev 解析json文件的依赖，需要手动在cfg/default.js文件下加入loader；
## 创建项目工程到完成项目踩过的坑
* 看别人或者视频项目，一定要注意用的版本号，旧版本和新版本有很大差别，会一直报错
* 比如 $ cnpm install sass-loader 可能后边需要加上版本号；
* 安装依赖时 $ cnpm install [依赖名字] --save-dev 可以直接将依赖版本加入到package.json文件，不需要再手动添加；
* 突然出现$ cnpm start时，出现错误，可能需要修改cfg/default.js文件下的端口号；
* 修改完后缀的.scss文件只能渲染html，body，不能渲染虚拟DOM的className时，可能是因为index.html下命名了一个class，并在.scss文件上，解决方案就是删除这个class；

