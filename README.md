### 개요
- spring boot + jsp file loading 테스트 프로젝트. 

### 설정 
- structure
```
├── pom.xml
├── src
│   ├── main
│   │   ├── java
│   │   │   └── net
│   │   │       └── joey
│   │   │           └── application
│   │   │               └── jspwork
│   │   │                   ├── JspworkApplication.java
│   │   │                   └── controller
│   │   │                       └── HelloController.java
│   │   ├── resources
│   │   │   └── application.properties
│   │   └── webapp
│   │       └── WEB-INF
│   │           └── jsp
│   │               └── hello.jsp

```

- pom.xml
```
    <dependency>
        <groupId>javax.servlet</groupId>
        <artifactId>jstl</artifactId>
    </dependency>
    <dependency>
        <groupId>org.apache.tomcat.embed</groupId>
        <artifactId>tomcat-embed-jasper</artifactId>
    </dependency>
```

- application.properties
```
	spring.mvc.view.prefix=/WEB-INF/jsp/
	spring.mvc.view.suffix=.jsp	
```

