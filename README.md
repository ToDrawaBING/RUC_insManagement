## 中国人民大学大型仪器管理平台 RUC_InsManagement



### 一、Introduction

本项目为数据库课程设计的前期demo版本，主要包括了该项目的前端设计、交互控制等内容。项目内容大致完整，基本只需要简单的命令就能够上手跑起这个网站。

本项目开源的初衷不是让师弟师妹们单纯把它当做一个cheatsheet，而是希望没有前端基础的师弟师妹们不要在这门课上把太多时间浪费在设计前端的内卷空耗里，把更多的时间精力放在数据库的性能设计（例如针对性的性能调优、并发控制等内容上），同时也能为想使用django开发简单网站的新手开发者提供一些帮助~

b站视频演示链接：https://www.bilibili.com/video/BV1CA411s7Q8/



### 二、配置环境 & 运行说明

#### 2.1. 配置环境需求

`python >= python3.7`

`Django >= 3.1.2`



#### 2.2. 运行说明

- **本项目的想法是提供一个干净易用的前端设计以及交互模式设计参考，让开发者把更多精力放在数据库性能设计上。因此，数据库方面只使用了django默认配置的sqlite；若开发者希望进一步开(mo)发(gai)，也可以轻松地利用框架迁移到mysql、postgre等数据库平台。**

- **轻松上手：进入目标文件夹，执行python manage.py runserver即可运行**

  - ```python
    cd RUC_insManagement
    python manage.py runserver	
    ```

    点击下方http://127.0.0.1:8000/即可进入主页啦~
    ![image](https://github.com/DengChenlong-Studio/RUC_insManagement/blob/master/readme_img/launch.png)




### 三、综合设计
#### 3.1. 登录首页（首页信息及轮播图等）
![image](https://github.com/DengChenlong-Studio/RUC_insManagement/blob/master/readme_img/homepage.JPG)


#### 3.2. E-R图

本项目的设计中主要有学生、老师、管理员三种角色，他们的关系可以由以下E-R图来展示：
![image](https://github.com/DengChenlong-Studio/RUC_insManagement/blob/master/readme_img/er_pic.png)


#### 3.3. 登录控制

登录方面提供了系统账号登录以及微人大登录两种方案，用户可以自由进行选择
1. 系统账号登录（数据库系统概论小彩蛋~）
![image](https://github.com/DengChenlong-Studio/RUC_insManagement/blob/master/readme_img/login1.png)

2. 微人大登录
![image](https://github.com/DengChenlong-Studio/RUC_insManagement/blob/master/readme_img/login2.png)

#### 3.4. 仪器预约控制

仪器预约提供了一站式的解决方案，学生用户可以在一个页面中进行仪器查看、仪器预约等操作：
![image](https://github.com/DengChenlong-Studio/RUC_insManagement/blob/master/readme_img/appointment.JPG)



#### 3.5. 仪器使用情况查看控制

为仪器管理员提供了仪器使用情况的月周日表查看机制，使相应用户能够使用这个功能进行统计以及情况打印：
![image](https://github.com/DengChenlong-Studio/RUC_insManagement/blob/master/readme_img/statistics.JPG)

