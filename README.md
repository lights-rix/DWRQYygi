# 前言

欢迎来到本项目的Gitee页面。本项目是一款基于Vue与Spring Boot的博客系统，适用于计算机专业毕业设计。这里将提供完整的源码、文档报告和代码讲解，以帮助您更好地理解和学习。接下来，让我们详细了解这个项目吧！

## 内容介绍

本项目是一个功能完善的博客系统，主要包括文章发布、评论、分类、标签等功能。前端使用Vue进行构建，实现了与后端Spring Boot的分离，提高了开发效率和项目的可维护性。通过这个项目，您可以学习到前后端分离的开发模式，以及如何使用Spring Boot和Vue实现一个完整的实战项目。

## 技术介绍

- **语言：** Java
- **使用框架：** Spring Boot
- **前端技术：** JS、Vue、css3
- **开发工具：** IDEA/Eclipse
- **数据库：** MySQL 5.7/8.0
- **数据库管理工具：** phpstudy/Navicat
- **JDK版本：** jdk1.8
- **Maven：** apache-maven 3.8.1-bin
- **前端环境：** Node.Js 12\14\16

## 核心代码

以下是项目中的一段核心代码，展示了如何使用Spring Boot接收前端传递的参数并返回数据。

```java
@RestController
@RequestMapping("/api/blog")
public class BlogController {

    @Autowired
    private BlogService blogService;

    @GetMapping("/list")
    public ResponseEntity<List<Blog>> list(@RequestParam("page") int page, @RequestParam("size") int size) {
        Pageable pageable = PageRequest.of(page, size);
        List<Blog> blogs = blogService.findAll(pageable).getContent();
        return ResponseEntity.ok(blogs);
    }
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img13.360buyimg.com/ddimg/jfs/t1/334137/11/10254/114960/68bc78bfF2a1dc552/82e80f25723526a0.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/344817/11/436/34639/68bc7898F3efde9d7/a0e726a6a6c766f4.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/338820/38/7728/66366/68bc7898Fb1e66179/ac3f3bb483aff4a6.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/350037/7/493/25992/68bc7899Febb0ed8f/3aef923ce4a47227.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/328207/11/17134/19430/68bc789aF5775b89a/7491cb7ffe423002.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/327558/19/16857/24374/68bc789aF67b93509/ff14c39d85b3f3c6.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/351220/11/461/27606/68bc789bF160d3bce/0163c226d0fcf40a.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/347356/30/490/45364/68bc789bF2bda942d/ce5d11cfae129325.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/333940/18/10162/47656/68bc789cF47916d8e/5630cb15ab6e5236.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/337971/32/7678/70687/68bc789dFb4a482e0/a95ebd168bff2fec.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
