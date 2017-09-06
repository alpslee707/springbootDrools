# springbootDrools
https://github.com/alpslee707/springbootDrools 项目文件

需要工具：
1.jdk1.7+

2.maven

3.drools包

4.eclipse

需要时间：
项目搭建时间10分钟+

使用技术spring boot + drools（7.0.0.final）

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



入门 DRL规则文件在when之前可以设置的属性如下所示：

no-loop：在DRL的then子句中，如果出现insert、update、modify、retract等方法对实例（Fact）做出修改时，当前规则执行完成后会触发该规则使其再执行一次；将no-loop设置为true则会强制规则在出现上述方法的情况下也只执行一次 boolean型，默认值为false

ruleflow-group：基于ruleflow将规则分组 string型，无默认值

lock-on-active：规则可能会被其它规则调用而反复执行；将lock-on-active置为true可以强制使规则在任何条件下都只会执行一次，可视为no-loop的加强版 boolean型，默认值为false

salience：设置当前这条规则的执行优先级，数字越小优先级越高 int型，默认值为0

agenda-group：基于Agenda将规则分组；只有当某个Agenda组获取到焦点（focus）时，该组的规则才会被执行 string型，默认值为MAIN

auto-focus：与agenda-group配合使用，设置焦点的是否可以自动获取 boolean型，默认值为false

activation-group：不基于任何条件将规则分组 string型，无默认值

dialect：设置规则所使用的语言 string型，默认值根据package值判断，值域为java或mvel

data-effective：当前规则的生效时间 string型，无默认值；值中需包含日期和时间

data-expires：当前规则的失效时间 string型，无默认值；值中需包含日期和时间

duration：设置DRL文件开始执行之后延迟多长时间开始执行这条规则 long型，无默认值



