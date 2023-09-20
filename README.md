# 传奇BI项目

说明：

基于Spring Boot+MQ+AIGC的智能数据分析平台。区别于传统Bl,用户只需要导入原始数据集、并输入分析诉求，就能自动生成可视化图表及分析结论，实现数据分析的降本增效。

## 启动步骤

### 导入数据库

在自己的电脑上导入数据库。

![image-20230920133749194](https://img2023.cnblogs.com/blog/2355908/202309/2355908-20230920140015488-1460141206.png)

### 后端

1.yubi-backend导入idea

2.修改鱼聪明的配置，替换成自己的

![image-20230920133649042](https://img2023.cnblogs.com/blog/2355908/202309/2355908-20230920140015085-655508534.png)

3.在本地启动redis和rabbitmq.

4.在yubi-backend\src\main\java\com\yupi\springbootinit\bizmq里面找到MqlnitMain,先启动

![image-20230920131702921](https://img2023.cnblogs.com/blog/2355908/202309/2355908-20230920140014584-1057130264.png)

5.启动springboot入口文件：MainApplication即可成功启动后端。

![image-20230920131900680](https://img2023.cnblogs.com/blog/2355908/202309/2355908-20230920140013967-1196166808.png)

### 前端

1.将malinbi-frontend导入webstorm或者vscode

2.安装依赖(我使用yarn,npm install报错了)

```
yarn
```

3.打开package.json，运行dev

4.可能会报错，安装echarts依赖

```
npm install echarts-for-react
```

进入界面后进行注册，然后使用账号和密码进行登录。



