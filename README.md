# kingTrap
## 只需要三个步骤既可以完成一个端口的监听了！！！真的是很强大！
- 打开IDEA2019，File->new Project,选择Spring Initializr创建工程；一直Next就可以了，点击Finish，自动生成HelloApplication.java类；
- 新建一个controller路径，创建HelloController.java,使用@RestController,并创建一个sayHello的方法，返回"Hello！", 使用@RequestMapping("/sayHello"),对方法进行映射;
- 在pom.xml中引入spring-boot-starter-web的依赖包，等自动加载jar包后，启动HelloApplication.java类

激动人心的时刻：打开浏览器，输入：http://localhost:8080/sayHello , 就可以访问了！

---

#### PS:中间有点小插曲，因为把HelloApplication.java放的目录跟controller同级，导致页面报404；这说明启动类必须在扫描路径的上一级目录才行！
