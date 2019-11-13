# smt-generator

### 项目介绍
+ 自动生成数据库表对应的java实体类、mapper接口、xml映射文件

+ 目前仅支持mysql、oracle数据库

### 使用说明
1. 选择对应的数据库连接驱动依赖包【pom.xml】
    
2. 更改数据库连接配置【db.properties】

3. 配置数据库对应的分页插件、元数据信息、需要映射的数据表等【generatorConfig.xml】

4. 使用mybatis-generator插件进行代码生成

### 注意事项
+ oracle数据库连接驱动不支持通过maven下载，需手动将其安装至本地版本库

+ 由于集成了部分自定义插件，首次使用前务必先执行"mvn clean install"命令将本项目安装至本地版本库，再使用mybatis-generator插件进行代码生成

### 扩展阅读
+ [MyBatis Generator官方文档](http://www.mybatis.org/generator/index.html)