jfinal-routebind
============

jfinal  route bind，查看其他插件-> [Maven](http://search.maven.org/#search%7Cga%7C1%7Ccn.dreampie)

maven 引用  ${jfinal-routebind.version}替换为相应的版本如:0.1

```xml
<dependency>
  <groupId>cn.dreampie</groupId>
  <artifactId>jfinal-routebind</artifactId>
  <version>${jfinal-routebind.version}</version>
</dependency>
```

使用非常简单

```java

/**
   * 配置路由
   */
public void configRoute(Routes routes) {
  RouteBind routeBind = new RouteBind();
  //排除扫描部分包
  //routeBind.addExcludePaths("cn.dreampie.exc");
  //扫描部分包
  //routeBind.addIncludePaths("cn.dreampie.inc");
  routes.add(routeBind);
}

```