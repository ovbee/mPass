<p align="center">
	<a href="http://mpass.gitee.io/zh-cn"><img src="https://images.gitee.com/uploads/images/2019/1009/235538_73450b95_1468963.png" width="700"></a>
</p>
<p align="center">
	<a target="_blank" href="https://search.maven.org/search?q=M-PasS">
		<img src="https://img.shields.io/badge/Maven Central-1.12.0-blue.svg" ></img>
	</a>
	<a target="_blank" href="https://gitee.com/ibyte/M-Pass/blob/master/LICENSE">
		<img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" ></img>
	</a>
        <a target="_blank" href="https://gitee.com/ibyte/M-Pass">
		<img src="https://img.shields.io/badge/Spring%20Boot-2.0.9.RELEASE-blue" alt="Downloads"/>
	</a>
        <a target="_blank" href="https://gitee.com/ibyte/M-Pass">
		<img src="https://img.shields.io/badge/Spring%20Cloud-Finchley.SR4-blue" alt="Downloads"/>
	</a>
	<a target="_blank" href="https://www.oracle.com/technetwork/java/javase/downloads/index.html">
		<img src="https://img.shields.io/badge/JDK-1.8+-green.svg" ></img>
	</a>
	<a target="_blank" href="https://gitee.com/ibyte/M-Pass" title="API文档">
		<img src="https://img.shields.io/badge/Api Docs-1.12.0-orange.svg" ></img>
	</a>
	 <a href='https://gitee.com/ibyte/M-Pass/stargazers'>
	    <img src='https://gitee.com/ibyte/M-Pass/badge/star.svg?theme=dark' alt='star'></img>
	 </a>
</p>

# mPass （Microservice Pass）
基于SpringBoot2.x、SpringCloud并采用前后端分离的企业级微服务,多租户系统架构微服务开发平台 mPaaS（Microservice PaaS）为租户业务开发、测试、运营及运维开源框架，能有效降低技术门槛、减少研发成本、提升开发效率，协助企业快速搭建稳定高质量的微服务应用;同时还集合各种微服务治理功能和监控功能。模块包括:企业级的认证系统、开发平台、应用监控、慢sql监控、统一日志、单点登录、Redis分布式高速缓存、配置中心、分布式任务调度、接口文档、代码生成等等

[TOC]

    ______  ___     ________                      
    ___   |/  /     ___  __ \_____ _______________
    __  /|_/ /________  /_/ /  __ `/_  ___/_  ___/
    _  /  / /_/_____/  ____// /_/ /_(__  )_(__  )
    /_/  /_/        /_/     \__,_/ /____/ /____/  

**作者**：iByte (码哥 or 李尚志)

## 如果您觉得有帮助，请点右上角 "Star" 支持一下谢谢

## 项目总体架构图
![项目架构图](https://images.gitee.com/uploads/images/2019/1018/020143_0d434b4a_1468963.jpeg "mPass_Springcloud微服务架构.jpg")

### 核心JAR架构依赖视图
![输入图片说明](https://images.gitee.com/uploads/images/2019/1009/000659_b0861629_1468963.png "JAR.png")

 :anger:  :facepunch:   _系统处于开发阶段, 预计**两个月**时间完成整体架构体系_

**核心功能**：
- **快速开发**：工程化的开发框架可以自动生成初始化代码，框架还提供模块化开发模式，适用于多人协作开发。
- **性能优化**：支持运营活动投放一站式全流程创建管理，加载智能化投放能力，最大可能提升运营效率和转化效果，助力业务增长。
- **数字化运营闭环**：所有组件都经历了高并发，大流量的检验，对弱网，保活，容器等都有深度的优化，能够兼容复杂的客户端情况
- **使用方式灵活**：框架与组件并没有强依赖，可分可合，灵活机动。各组件可以独立的提供强大的功能，也可以互相配合优化使用体验，发挥更大的作用

### maven 主要核心包版本依赖
- **目前架构支持 H2database | MySQL | Oracle  | Sqlserver  四种数据库的切换，用户可自由选择安装数据库**

|  依赖包   | 说明    |
| --- | --- |
|  JDK   | 1.8   |
|  Spring-Cloud   |  Greenwich.SR2   |
|  Spring-Boot   |   2.1.6.RELEASE  |
|  Spring-Boot-admmin   |  2.1.6   |
|  druid   |  1.1.10   |
|  netty-all   |  RELEASE   |
|  h2database   |  1.4.197   |
|  mysql   |  5.1.46   |
|  oracle   |  12.1.0.1.0   |
|  sqlserver   |  6.0.8112.200   |
|  arangodb   |  4.2.2   |
|  elasticsearch   | 6.1   |
|  jedis   |  2.9.0   |
|  logstash   |  6.1   |
|  guava   |  20.0   |
|  reflections   |  0.9.11   |
|  swagger2   | 2.9.2  |
|  lombok   | 1.18.8  |

**查看更新记录请移步**
[目前进度](https://gitee.com/ibyte/M-Pass/blob/master/UPDAT-RECORD.md)
- [x] common
    - [x] common-base
    - [x] common-api 
    - [x] common-core
- [x] framework-discovery
    - [x] framework-discovery-api
    - [x] framework-discovery-client
    - [x] framework-discovery-core
    - [x] framework-plugin-api
    - [x] framework-plugin-client
    - [x] framework-plugin-core
- [x] framework-gateway
    - [ ] framework-gateway-api
    - [ ] framework-gateway-core
- [x] sys-job
    - [ ] sys-job-api
    - [ ] sys-job-client
    - [ ] sys-job-core
## 项目部分展示图
<table>
    <tr>
        <td><img src="https://images.gitee.com/uploads/images/2019/1023/105813_2678586b_1468963.png"/></td>   
        <td><img src="https://images.gitee.com/uploads/images/2019/1023/105813_42dbd65f_1468963.png"/></td>
    </tr>
    <tr>
        <td><img src="https://images.gitee.com/uploads/images/2019/1023/105750_536c2d49_1468963.jpeg"/></td>   
        <td><img src="https://images.gitee.com/uploads/images/2019/1023/105813_12560953_1468963.jpeg"/></td>
    </tr>
    <tr>
        <td><img src="https://images.cnblogs.com/cnblogs_com/lishangzhi/1573128/o_权限组织管理.png"/></td>
        <td><img src="https://images.cnblogs.com/cnblogs_com/lishangzhi/1573128/o_日志管理.png"/></td>
    </tr>
</table>
## 1.1 开发细节
### 1.1 SPI拓展
**SpringBoot SPI拓展**
- 支持自定义Banner拓展
- 支持设置默认config配置文件加载
- 支持实现logback拓展
- 支持实现redis拓展
- 支持实现spring基础拓展

```java
org.springframework.boot.SpringApplicationRunListener=\
  com.ibyte.component.config.DefaultConfigListener,com.ibyte.component.logback.LogbackListener,com.ibyte.component.banner.BannerListener
org.springframework.boot.autoconfigure.EnableAutoConfiguration=\
  com.ibyte.component.spring.PackageScanAutoConfig,com.ibyte.component.redis.RedissonAutoConfiguration
com.ibyte.component.config.DefaultConfigFactory=\
  com.ibyte.component.config.InitPropConfigFactory
```
## 1.2 IDGenerator
**ID生成器**
```java
/**
 * 生成主键，36位，[0-9a-w]：时间+w+jvmId+w+流水号+w+随机数填充+w+tenantId
 */
public static String generateID() {
    return generateID(System.currentTimeMillis(), TenantUtil.getTenantId());
}
/**
 * 根据指定时间生成主键
 */
public static String generateID(long time) {
    return generateID(time, TenantUtil.getTenantId());
}

/**
 * 根据指定时间，租户生成主键
 */
public static String generateID(long time, int tenant) {
    StringBuilder id = new StringBuilder(LEN);
    id.append(Long.toUnsignedString(time, 32)).append(SPLIT)
            .append(Long.toUnsignedString(jvmId, 32)).append(SPLIT);
    String tenantId = Integer.toUnsignedString(tenant, 32);
    // 除去租户ID长度
    int length = LEN - tenantId.length() - 1;
    // 序列号填充，若填充完超过指定长度，则取后半部分
    String seqNum = Long.toUnsignedString(SEQ.incrementAndGet(), 32);
    if (id.length() + seqNum.length() > length) {
        seqNum = seqNum.substring(id.length() + seqNum.length() - length,
                seqNum.length());
    }
    id.append(seqNum).append(SPLIT);
    // 随机数填充，不超过leng长度
    while (id.length() < length) {
        id.append(Integer.toUnsignedString(RANDOM.nextInt(), 32));
    }
    id.delete(length, id.length());
    return id.append(SPLIT).append(tenantId).toString();
}
```
### 1.3 异常国际化处理
**RuntimeException 拓展类处理**
```java
public KmssRuntimeException(String messageKey) {
		super(ResourceUtil.getString(messageKey));
		this.code = messageKey;
}
```
### 1.4 本地扩展点
```java
/**
 * 本地扩展点的声明采用注解的方式声明，并在注解上使用LocalExtensionPoint的注解<br>
 *
 * <li>若定义了manager类，插件工厂在初始化时会自动往manager中注入Provider的信息，configurable强制为false。</li>
 * <li>若定义了config类，则Plugin.getProvider的class参数为config，返回值为config类的实例。</li>
 * <li>若未定义了config类，但定义了baseOn，则Plugin.getProvider的class参数为baseOn，返回值为注解所在类的实例（优先Spring的Bean）。</li>
 * <li>未定义config，未定义baseOn，则扩展点无效</li>
 *
 * @author li.Shangzhi
 * @Date: 2019-10-17
 */
@Target({ ElementType.ANNOTATION_TYPE })
@Retention(RetentionPolicy.RUNTIME)
public @interface LocalExtensionPoint {
   //...
}
```
### 1.5 系统内置配置
**@EnableConfigurationProperties 与 @ConfigurationProperties 处理**
```java
@Configuration
@EnableConfigurationProperties({SystemConfig.class, TenantConfig.class, LicenseConfig.class, LanguageConfig.class, CorsConfig.class})
```
```java
// 多语言配置信息
@ConfigurationProperties("kmss.lang")
public class LanguageConfig {
    //...
}

// 系统配置
@ConfigurationProperties("kmss.system")
public class SystemConfig {
    //...
}
```
**交流群**
<table border="0">
    <tr>
        <td>QQ交流群：(877056205) mPaaS</td>
        <td>微信交流群：微信群(加微信入群)</td>
        <td>微信公众号：码农架构</font></td>
    </tr>
    <tr>&nbsp;</tr>
    <tr>
        <td><img title="QQ交流群-877056205" src="https://images.gitee.com/uploads/images/2019/1023/154958_d9571f28_111383.png" height="200" width="200"/></td>
        <td><img title="微信交流群" src="https://images.gitee.com/uploads/images/2019/1023/154754_6cc08ffd_111383.png" height="200" width="220"/></td>
        <td><img title="微信公众号-微技术栈" src="https://images.gitee.com/uploads/images/2019/1023/155117_006731a8_111383.jpeg" height="200" width="200"/></td>
    </tr>
</table>
