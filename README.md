#hihsoft-atomikos
【组件价值】

Atomikos 是一款 Java/JTA 事务处理工具

与spring完美结合，实现配置化分布式事务

多数据源分布式事务的开源解决方案

跨平台，不受应用服务器限制

也是学习spring、mybatis、junit技术整合不可多得的实践案例

【组件定位】

 Atomikos中文资料比较少，网上的资料大多都是千篇一律，抄袭成风，误人不浅

HihSoft-atomikos以组件案例的形式展现，降低Atomikos的学习和使用门槛

【面向业务】

  主要是有分布式事务，又不想使用EJB的多数据库操作的业务系统。

【组件技术】

Spring Framework 3.2

mybatis

Atomikos

Junit

【框架特点】

 精简、通俗易懂

源于实践项目提纯，实用性强

【组件源码说明】


 包    说明
com.hihframwork.core.baseclass	封装与mybatis,spring交互的持久化基类
├ domain	域对象基类
├ persistence	封装与mybatis,spring交互的持久化基类
├ service	封装业务逻辑层基类
com.hihframwork.core.utils	各种工具类
com.hihframwork.exception	异常类
com.hihsoft.db1	分布式事务用例中用到的数据库DB1
├ domain	子系统域对象
├ persistence	子系统持久化类及接口
├ service	子系统业务层服务
com.hihsoft.db2	分布式事务用例中用到的数据库DB2
├ domain	岗位域对象
├ persistence	岗位持久化类及接口
├ service	岗位业务层服务
resources\resources	配置文件
├springcfg	mybatis,atomikos,spring相结合的配置文件
├dbcfg	不同数据库的表结构脚本
jdbc.properties	与数据库相关的驱动设置及数据库配置文件
log4j.xml	工程日志文件log4j
test	junit测试目录
com.hihsoft.system.service	本组件测试用例，具体见代码
com.hihsoft.util	测试基类