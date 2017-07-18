# springbootDrools
drools.rar 项目文件，解压导入到eclipse使用

1.jdk1.7+

2.maven

3.drools包

项目搭建时间10分钟+

使用技术spring boot + drools

需要下载eclipse插件：
1.drools-distribution-7.0.0.Final.zip 
这个是在eclipes中添加drools运行环境。

2.droolsjbpm-tools-distribution-7.0.0.Final.zip
这个是在eclipse中可以添加drools项目使用。

配置方法：
1将drools-distribution-7.0.0.Final.zip  解压。准备


2将droolsjbpm-tools-distribution-7.0.0.Final 解压。
将binaries\org.drools.updatesite\plugins 下的所有jar包复制到
eclipse\plugins 下面

3接下来重启eclipse

4找到菜单window-prefences 找到 drools 插件。选择installed Drools Runtimes。

5右侧add 选择路径 drools-distribution-7.0.0.Final.zip 解压的地址 drools-distribution-7.0.0.Final\binaries

6重启eclipse

ok插件安装完毕。

7把项目导入到eclipse下载jar包。然后java run  DroolsService.java 就可以体验 drools规则引擎了。


