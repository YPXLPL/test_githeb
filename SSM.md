- controller:在controller里面放的是界面控制器，主要写每个界面对应的功能，相当于程序的核心区，通过调用业务层service接口中的方法来实现。@Controller来源于@Component，表示为控制层，用于加在类上，同理，@Repostirory加在DAO层，@Service加在服务层。@RequestMapping("getHome")该方法对应的uri;根据返回的字符串找到对应的视图。
- intercepter:拦截器 创建一个拦截器实现接口HandlerInterceptorAdapter,在springmvc的核心配置文件中添加该拦截，拦截并解析请求头中的环境语言，设置服务器端的语言环境，从而实现服务器端响应内容的国际化。
- mapper:Mybatis里面的mapper和xml的语句映射，是针对SQL构建的，如果拿他跟具有相同功能的JDBC代码进行对比，可以省略将近95%的代码、if、choose、where、set、foreach、bind、script等元素的作用。
- pojo:pojo中存放的是实体类，使用POJO类型进行数据绑定。
- service:service类是主要的功能开发的地方，具体来说就是在service接口中编写方法，不需要具体实现，在serviceimpl中来实现service接口，并且return mapper中的方法来实现功能，使用的时候直接调用service就可以了。



- mybatis-config.xml:Mybatis的配置文件包含了设置(Settings)和属性(properties)信息。setting是调整设置，它们会改变Mybatis的运行时行为。properties：这些属性都是可外部配置且可动态替换的，既可以在Java属性文件中配置，也可以通过properties元素的子元素来传递。
- applicationContext.xml:
- dispatcherServlet-servlet.xml:
- jdbc.properties:
- log4j.properties:日志系统的配置文件