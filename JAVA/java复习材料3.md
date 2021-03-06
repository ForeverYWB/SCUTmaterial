1. **Java 程序是由什么组成的？一个程序中必须有 public 类吗？ Java源文件的命名规则是怎么样的？**
答：一个Java程序是有若干个类组成。一个Java程序不一定需要有public类：如果源文件中有多个类时，则只能有一个类是public类；如果源文件中只有一个类，则不将该类写成public也将默认它为主类。源文件命名时要求源文件主名应与主类（即用public修饰的类）的类名相同，扩展名为.java。如果没有定义public类，则可以任何一个类名为主文件名，当然这是不主张的，因为它将无法进行被继承调用。另外，对Applet小应用程序来说，其主类必须为public，否则虽然在一些编译平台下可以通过（在BlueJ下无法通过）但运行时无法显示结果。
<br><br>
2. **怎样区分应用程序和小应用程序？应用程序的主类和小应用程序的主类必须用 public 修饰吗？**
答：Java Application 是完整的程序，需要独立的解释器来解释运行；而 Java Applet 则是嵌在HTML编写的 web 页面中的非独立运行程序，由 web 浏览器内部包含的 Java 解释器来解释运行。
在源程序代码中两者的主要区别是：任何一个 Java Application 应用程序必须有且只有一个 main 方法，它是整个程序的入口方法；任何一个 Applet 小程序要求程序中有且必须有一个类是系统类 Applet 的子类，即该类头部分以 extends Applet 结尾。
应用程序的主类当源文件中只有一个类时不必用 public 修饰，但当有多于一个类时则主类必须用 public 修饰。小应用程序的主类在任何时候都需要用 public 来修饰。
3. **开发与运行 Java 程序选哦经过哪些主要步骤和过程？**
答：主要有三个步骤
* 用文字编辑器 notepad （或其它编辑器）编写源文件；
* 使用 Java 编译器（如 Javac.exe )将.java源文件编译成字节码文件.class；
* 运行 Java 程序：对应用程序应通过 Java 解释器（如 java.exe ）来运行，而对小应用程序应通过支持 Java 标准的浏览器（如 Microsoft Explorer）来解释运行。
4. **安装 JDK 之后如何设置 JDK 系统的 PATH，CLASSPATH？他们的作用是什么？**
答：更新系统PATH的方法随 Windows 版本不同而不同。对于 Windows 95/98，可以将下列项目作为C:\autoexec.bat的最后一行：
SET PATH = C:\j2sdk1.4.2\bin;%PATH%
当程序需要第三方的类库支持，而且比较常用，就可以采用此种方法。比如常用的数据库驱动程序，写 servlet 需要的 servlet 包等等，设置方法就是在环境变量中加入CLASSPATH，然后就可以直接编译运行了。Java 运行环境从 CLASSPATH 环境变量中寻找要执行的用户项目（三方的类库）。可以按如下的方式设置：
SET CLASSPATH = .;C:\J2SDK1.4.2\jre\lib\jaws.jar;%CLASSPATH%
通常我们要从当前目录寻找用户类，因为开发的程序相关的类放在这里，.表示当前的工作目录。
5. **Java语言特点是什么？**
答：Java是一种简单的面向对象的分布式的解释的健壮的安全的结构中立的可移植的性能很优异的多线程的动态的语言。
![](https://upload-images.jianshu.io/upload_images/15206312-e3ef107113b0cae5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-0ebfbee920c37ef0.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-418a62be77204a78.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-2b6e92090daa504d.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-16d54726d4ec5c8b.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-54e05b7b886b71a5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-bfd408e72bd33916.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-36384112673167c8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-51e6e1e47a8fe97f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-ad28f781af47fba5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-9936e633b00adf8b.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-89208825b8281169.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-1031a0894402e1ee.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-cab6685e91706788.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-00d1bbf60c4e2445.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/15206312-5d06546a7fc989e1.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
