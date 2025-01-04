---
source: https://www.bilibili.com/video/BV14z4y1N7
date: 2024-06-19
tags: 
up:
---
# 基础篇

### bean注册

如果要注册的bean来自第三方，无法使用@component声明bean

这时使用@import 来导入 config类      
### 自动配置原理

- 主启动类上添加的注解组合了"enableAutoConfiguration"注解
-  "enableAutoConfiguration"注解通过import导入了"AutoConfigurationImportselector"
- 实现selectImports方法，最终读取Meta-INF目录下的. imports文件（或者spring. factories）文件
- 读取文件里的全类名，并解析了注册条件，把满足注册条件的Bean对自动注入到IOC容器中
 
# 实战篇
