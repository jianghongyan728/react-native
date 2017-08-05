## react-native的配置
##### 首先要把安卓的环境搭上，才可以运行react-native，接下来我就把我的搭环境的步骤写在下面
###### 这两个都可以安装，我的电脑是64位的，安装完之后就要配置环境变量了
- java环境的搭建
1. JDK的安装，我把我网盘的链接给大家，直接去下载就可以
http://pan.baidu.com/s/1dFvknT3   密码是n1x6，

2.  JAVA_HOME   环境变量的设，就是你jdk安装的位置
3.  修改环境变量path  环境变量，%JAVA_HOME%/bin;加在path的前面，千万别把原来的覆盖，要粘贴在原来基础上的最前面
4.  修改环境变量classpath，%JAVA_HOME%/lib/dt.jar;%JAVA_HOME%/lib/tools.jar
5. 验证

```
java -version//查看版本
javac//查案环境变量是否配置成功
```
- android环境的搭建
##### 配置完java的环境，接下来就配置android的环境
1. sdk的安装
2. eclipse或者android-studio安装这两个都可以，我安装的是eclipse
http://pan.baidu.com/s/1bA9oqM   密码plr4
3. ANDROID_HOME环境变量的设置,就是你sdk安装的位置
4. 修改环境变量path  环境变量
%ANDROID_HOME%/tools;%ANDROID_HOME%/platform-tools;
把这句加在path，java环境的后边就可以了
5. 验证

```
android//在黑框里输入android出来东西就证明你安6装成功了
```
##### 配置完安卓的环境，接下来就安装react-native
- reactnative 的安装
1. 安装Node.js
2. Python2

```javascript
http://pan.baidu.com/s/1o7Vj5Z8   密码i9xo
去下载吧，32位的和64位的都有
node -v //查看node的版本
	
python -V //查看python的版本，python的-V必须是大写的V
```
3. npm install -g react-native-cli//安装react-native

```
如果安装的慢，也可以用淘宝的镜像

npm config set registry https://registry.npm.taobao.org --global
npm config set disturl https://npm.taobao.org/dist --global
```
4. react-native init test创建文件
5. cd test跳转创建的文件夹下
6. 连接设备（我用的真机）
7. react-native run-android运行结果
- 真机器调试
1. 关于手机 -软件版本号
2. 更多设置 -开发者选项-usb调试
3. adb devices （装豌豆荚）手机电脑都装，也可以不装，只要手机电脑能连上就可以

##### 运行的时候会遇到很多坑，坑的会让人发疯，哈哈哈！！！！
1. 报错1

```
You have not accepted the license agreements of the following SDK components:

如果遇到这个错不要慌，按我说的就会解决

拷贝  licenses 到 android\sdk

我把这个文件的链接给大家

http://pan.baidu.com/s/1pLujYkz    密码buoc
```
2. 报错2

```
Error while uploading app-debug.apk : Unknown failure ([CDS]close[0])

不要慌，不要慌，条的坑多了，也就顺其自然了

https://stackoverflow.com/questions/39518928/gradle-error-while-uploading-app-local-debug-apk-unknown-failure-cdsclose
```
3. 报错3

###### 这个错是在运行到手机上出的错，然后按照下面的图片做，在运行就ok了
![image](D:\jj.png)

4. 报错4

> 这个错就说你少android-23

> 你在黑框上输入android就会出来一个框，然后把android-23下载上，在运行就可以了



##### 以上就是我所遇到的所有坑， 希望可以帮到大家










