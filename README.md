# hotel-vue
这是bro用一天时间写出来的一个基于SpringBoot+Vue3+MySQL9.0+MyBatis的酒店预定管理系统，包括前台和后台。已经实现基本的前后台功能模块，像后端里面已经写了一些比如说富文本编辑器，文件上传下载的接口，paotman已经测试好了接口能用，目前前端还没有完善这些功能，也没有考虑到使用redis等非关联数据库，消息队列啥的暂时，用来练速度的项目。因为Bro最近事情比较多，后面再逐步添加一些技术栈完善完善该项目。
hotel_booking.sql为数据库文件，管理员账号admin,密码123456。普通用户test@example.com，密码123456。暂未使用MD5等对密码加密。
前端npm install下载架包然后运行npm run dev即可。

使用技术：
### 后端技术栈
1. 核心框架 ：
   - Spring Boot 3.2.10
   - Java JDK 17
2. 持久层 ：
   - MyBatis + MyBatis-Spring-Boot-Starter 3.0.3
   - PageHelper 分页插件 1.4.6
   - MySQL Connector/J
3. 安全认证 ：
   - JWT (jjwt 0.12.5)
4. 工具库 ：
   - Lombok 1.18.30
   - Hutool 5.8.25
   - Apache POI 5.3.0 (Excel操作)
5. 其他支持 ：
   - Spring Validation (数据校验)
   - Spring Data Redis
   - Spring AOP
   - Commons FileUpload 1.5 (文件上传)
### 前端技术栈 (根据package.json)
1. 核心框架 ：
   - Vue 3
   - Vue Router 4
2. UI组件库 ：
   - Element Plus 2.8.4
3. 工具库 ：
   - Axios 1.7.7 (HTTP请求)
   - ECharts 5.5.1 (图表)
   - WangEditor 5.1.23 (富文本编辑器)
4. 构建工具 ：
   - Vite 5.3.1

### 项目结构说明
1. 后端(springboot) ：
   
   - src/main/java ：Java源代码
   - src/main/resources/mapper ：MyBatis映射文件
   - src/main/resources/application.yml ：配置文件
2. 前端(hotel-vue) ：
   
   - src/views ：页面组件
   - src/front ：前台页面相关
   - src/utils ：工具类

运行截图如下：
后台：
![微信图片_2025-06-23_112028_032](https://github.com/user-attachments/assets/902627b3-ee76-4b1d-8426-e2f85f96dbf2)
![图片1](https://github.com/user-attachments/assets/8cc7aee6-57e7-469d-87d7-86327ce5bcd3)
![微信图片_2025-06-23_112038_906](https://github.com/user-attachments/assets/c85ade74-d700-498c-b134-a2763217ff38)
前台：
![图片3](https://github.com/user-attachments/assets/f3d9d9af-dd3b-45a9-a6da-c33c7f2d3dd8)
![图片2](https://github.com/user-attachments/assets/f7047588-24d5-4654-9655-ba3669ad7247)

代码文件附：
完整的软件测试文档，包括Jmeter性能测试

