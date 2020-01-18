

# Spring源码

## 一、spring架构

![spring架构](E:\Typero_workspace\spring\pic\Snipaste_2020-01-18_20-45-38.png)

## 

## 二、spring 环境（上下文）初始化

## 1、spring环境初始化相关类

![spring环境初始化](E:\Typero_workspace\spring\pic\Snipaste_2020-01-18_21-09-19.png)

其他的实体类继承`AbstractApplicationContext`抽象类

## 2、触发初始化的几种方式

- ```java
  // 解析配置文件
  ClassPathXmlApplicationContext cpac = new ClassPathXmlApplicationContext();
  ```

- ```java
  // 使用注解扫描
  AnnotationConfigApplicationContext acac = new AnnotationConfigApplicationContext();
  ```

- ```java
  // 文件系统中加载配置(不常用)
  FileSystemXmlApplicationContext fsac = new FileSystemXmlApplicationContext();
  ```

## 3、Bean初始化

- 读取bean，解析bean，实例化bean，将bean注册到spring环境中

- BeanFactory实现类

  ![DefaultListableBeanFactory](E:\Typero_workspace\spring\pic\Snipaste_2020-01-18_22-26-10.png)

