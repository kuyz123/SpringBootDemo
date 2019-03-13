# SpringBootDemo

    
Spring Boot 学习示例
=========================

![Spring Boot 2.1.3.RELEASE](https://img.shields.io/badge/Spring%20Boot-2.1.3.RELEASE-brightgreen.svg)
![Mysql 5.6](https://img.shields.io/badge/Mysql-5.6-blue.svg)
![JDK 1.8](https://img.shields.io/badge/JDK-1.8-brightgreen.svg)
![Maven](https://img.shields.io/badge/Maven-3.6.0-yellowgreen.svg)
![license](https://img.shields.io/badge/license-MPL--2.0-blue.svg)  


## 介绍
收集记录学习spring的点点滴滴，通过每一个小demo，一步步进阶，逐步完善。

实际开发过程很少碰到单模块的项目，所以该项目使用多模块开发，更贴合实际开发要求。
所以检出项目时请检出整个目录，而不是只检出某个demo。

当然考虑到多模块加载依赖问题，也可以只检出某个模块的demo，只是运行前请更改子模块pom.xml:

更改前：
```
    <parent>
        <groupId>com.mrcoder</groupId>
        <artifactId>SpringBootDemo</artifactId>
        <version>1.0.0</version>
        <relativePath>../pom.xml</relativePath>
    </parent>
```

更改后：

```
    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>2.1.3.RELEASE</version>
        <relativePath/> <!-- lookup parent from repository -->
    </parent>
```

## 子模块简写

sb    =》 spring boot

sbm   =》 spring boot mybatis

sbmp  =》 spring boot mybatis plus


## 案例

- [sb-helloword](https://github.com/MrCoderStack/SpringBootDemo/tree/master/sb-helloword)：IDEA创建spring boot项目
- [sb-jpa](https://github.com/MrCoderStack/SpringBootDemo/tree/master/sb-jpa)：jpa方式访问mysql
- [sbm-annotations](https://github.com/MrCoderStack/SpringBootDemo/tree/master/sbm-annotations)：注解方式访问mysql
- [sbm-generator](https://github.com/MrCoderStack/SpringBootDemo/tree/master/sbm-generator)：mapper.xml方式操作数据，mybatis-generator-maven-plugin自动生成代码，集成pagehelper-spring-boot-starter分页控件来使用，附带非分页方式
- [sbmp-multidb](https://github.com/MrCoderStack/SpringBootDemo/tree/master/sbmp-multidb)：mapper.xml方式访问mysql，mybatis-plus-generator自动生成代码，dynamic-datasource-spring-boot-starter多库切换
- [sbmp-multidb-druid](https://github.com/MrCoderStack/SpringBootDemo/tree/master/sbmp-multidb-druid)：注解方式访问mysql，spring-boot-starter-aop，druid多库切换







