### 注解
声明Bean的注解：
    @component组件，没有明确的角色。
    @Service在业务逻辑层（Service层）使用。
    @Repository在数据访问层（Dao层）使用。
    @Controller在展现层（MVC→Spring MVC）使用。
注入Bean的注解：一般情况下通用。
    @Autowired：Spring提供的注解。
    @Inject：JSR-300提供的注解。
    @Resource：JSR-250提供的注解。
    @Autowired、@Inject、@Resource可注解在set方法上或者属性上，笔者习惯注解在属性上，有点是代码更少，层次更清晰。
