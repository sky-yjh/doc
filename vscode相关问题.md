### python输出中文为乱码

<img src="C:\Users\18857\AppData\Roaming\Typora\typora-user-images\image-20220901225848717.png" alt="image-20220901225848717" style="zoom: 67%;" />

使用code_runner运行py代码时输出出现中文乱码

- 原因：code_runner存在编码问题
- 解决方案：通过设置打开settings.json文件

<img src="C:\Users\18857\AppData\Roaming\Typora\typora-user-images\image-20220901230338216.png" alt="image-20220901230338216" style="zoom: 50%;" />

在其中添加`set PYTHONIOENCODING=utf-8 && python `

![image-20220901230450754](C:\Users\18857\AppData\Roaming\Typora\typora-user-images\image-20220901230450754.png)