# spring-boot-vue

#### 项目介绍

#### 软件架构
com.example.demo ：api项目springboot REST API </br>
com.example.demo.client： web前端项目 vue+vue-router+axios+webpack


#### 运行

进入api项目运行springboot 项目，在浏览器地址输入：http://localhost:8081/index.html

#### 开发

进入web目录执行如下命令

#### 安装依赖

npm install

#### 在 localhost:8002 启动前端项目

npm run dev</br>

由于我在web项目中已经配置了端口转发，将数据转发到SpringBoot上，因此项目启动之后，在浏览器中输入 http://localhost:8002 就可以访问我们的前端项目了，所有的请求通过端口转发将数据传到SpringBoot中（注意此时不要关闭SpringBoot项目）。
PS：关于端口转发和前端项目测试时候的端口修改，请查看 com.example.demo.client/config/index.js文件

#### 上线

npm run build</br>

该命令执行成功之后，api目录com.example.demo\src\main\resources\static下将生成页面所需要的脚本。
最后就可以将项目发布到开发、生产环境中了
