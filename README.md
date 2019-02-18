# BlockingForMyProject
Android 模块化样例，参见：https://www.jianshu.com/p/8b6e6a50e21e

传统项目缺点：
1、随着项目的增大，项目逐渐失去层次感，别人接手时吃力
2、我们在debug一个小功能的时候每次修改代码都需要重新build整个项目，这样显的很不合理
3、多人联合开发在版本管理中很容易出现冲突和代码覆盖的问题

搭建组件化模块步骤：
1、创建项目（即app模块），添加基础模块（commonLib模块），按照功能划分各个业务组件模块（以微信为例可以划分为：chat，contract，find，mine四大模块）
2、设置模块之间的依赖：通过配置gradle解决。
3、实现各业务模块之间的页面跳转以及通信：使用ARouter实现。

TODO:
  <1>创建基类；
  <2>使用dagger2+RxJava+Retrofit+RxAndroid+Glide，构建一个mvp框架；
