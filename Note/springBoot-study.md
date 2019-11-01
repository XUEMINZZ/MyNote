# 一、注解：
##  @Entity注解加在实体类上，定义对象将会成为被JPA管理的实体，将映射到指定的数据库。
##  @Id
##  @GeneratedValue(strategy=GenerationType.AUTO)
### 以上两个注解加在属性上，说明该字段是实体得唯一标识，并且这个字段的值是自动生成的（由属性GenrationType确定）
##  @Controller 用在类上，将其定义成一个控制器类
##  @RequestMapping 来映射URL到控制器类，或者是到Controller控制器的处理方法上。当@RequestMapping标记在Controller类上的时候,
## 里面使用@RequestMapping标记的方法的请求地址都是相对于类上的@RequestMapping而言的；
## 当Controller类上没有标记@RequestMapping注解时，方法上的@RequestMapping都是绝对路径。
## 这种绝对路径和相对路径所组合成的最终路径都是相对于根路径“/”而言的
