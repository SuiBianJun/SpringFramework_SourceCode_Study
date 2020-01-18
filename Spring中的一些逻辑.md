1、Bean存放在BeanFactory中，Spring的环境应该持有BeanFactory实例

```java
class GenericApplicationContext {
    private final DefaultListableBeanFactory beanFactory;
}
```

![GenericApplicationContext](E:\Typero_workspace\spring\pic\Snipaste_2020-01-18_22-46-56.png)



2、Bean如何放入BeanFactory的Map中的