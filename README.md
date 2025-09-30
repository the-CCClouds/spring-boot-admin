# Spring Boot Admin by [codecentric](https://codecentric.de)

> 本项目基于 [spring-boot-admin](https://github.com/codecentric/spring-boot-admin) 搬运，遵循其开源协议（Apache-2.0）。

> 这个项目不是一个完整业务系统，而是提供监控/管理界面，用来管理 Spring Boot 应用，包括通过 Actuator 暴露的健康状态、度量指标（metrics）、日志等功能。适合用于运维／监控／后台工具类用途。

> 如果你的需求里有监控、管理界面这样的部分，这个项目可以直接拿来用或参考。它可以作为一个子系统嵌入你的整体系统中。

[![Apache License 2](https://img.shields.io/badge/license-ASF2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0.txt)
![Build Status](https://github.com/codecentric/spring-boot-admin/actions/workflows/build-main.yml/badge.svg?branch=master)
[![codecov](https://codecov.io/gh/codecentric/spring-boot-admin/branch/master/graph/badge.svg?token=u5SWsZpj5S)](https://codecov.io/gh/codecentric/spring-boot-admin)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/de.codecentric/spring-boot-admin/badge.svg)](https://maven-badges.herokuapp.com/maven-central/de.codecentric/spring-boot-admin/)
[![Gitter](https://badges.gitter.im/codecentric/spring-boot-admin.svg)](https://gitter.im/codecentric/spring-boot-admin?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

这是一个社区项目，它为 [Spring Boot <sup>®</sup>](http://projects.spring.io/spring-boot/ "Official Spring-Boot website") Web 应用提供了一个管理界面，用于暴露 actuator 端点。

对于 Python 应用，可以使用 [Pyctuator](https://github.com/SolarEdgeTech/pyctuator)进行监控。

## 兼容性矩阵
在 Spring Boot Admin Server 应用中，Spring Boot Admin 的版本与 Spring Boot 的主版本和次版本保持一致。

| Spring Boot 版本    | Spring Boot Admin |
|---------------------|-------------------|
| 2.7                 | 2.7.Y             |
| 3.0                 | 3.0.Y             |
| ...                 | ...               |
| 3.3                 | 3.3.Y             |

不过，也可以独立于底层 Spring Boot 版本来监控任意版本的 Spring Boot 服务。
因此，可以运行 Spring Boot Admin Server 2.6 来监控一个运行在 Spring Boot 2.3 上的服务（通过 Spring Boot Admin Client 2.3）。

## 快速开始

你可以在官方文档中找到一份[快速指南](https://docs.spring-boot-admin.com/current)。

YouTube 上也有一些介绍视频：

<a href="https://youtu.be/Ql1Gnz4L_-c" target="_blank"><img src="https://i.ytimg.com/vi/Ql1Gnz4L_-c/maxresdefault.jpg"
alt="Cloud Native Spring Boot® Admin by Johannes Edmeier @ Spring I/O 2019" width="240" height="135" border="10" /></a><br>
**Cloud Native Spring Boot® Admin by Johannes Edmeier @ Spring I/O 2019**

<a href="https://youtu.be/__zkypwjSMs" target="_blank"><img src="https://i.ytimg.com/vi/__zkypwjSMs/maxresdefault.jpg"
alt="Monitoring Spring Boot® Applications with Spring Boot Admin @ Spring I/O 2018" width="240" height="135" border="10" /></a><br>
**Monitoring Spring Boot® Applications with Spring Boot Admin @ Spring I/O 2018**

<a href="https://goo.gl/2tRiUi" target="_blank"><img src="https://i.ytimg.com/vi/PWd9Q8_4OFo/maxresdefault.jpg"
alt="Spring Boot® Admin - Monitoring and Configuring Spring Boot Applications at Runtime" width="240" height="135" border="10" /></a><br>
**Spring Boot® Admin - Monitoring and Configuring Spring Boot Applications at Runtime**

## 获取帮助

使用 codecentric 的 Spring Boot Admin 遇到问题？我们愿意提供帮助！

 * 查看[参考文档](http://codecentric.github.io/spring-boot-admin/current/)。

 * 在[stackoverflow.com](http://stackoverflow.com/questions/tagged/spring-boot-admin)上提问（我们会关注`spring-boot-admin`标签的问题）。

 * 在[spring-boot-admin Gitter 聊天室](https://gitter.im/codecentric/spring-boot-admin)寻求帮助。

 * 在GitHub上提交bug： http://github.com/codecentric/spring-boot-admin/issues。

## 商标与许可证
codecentric 的 Spring Boot Admin 源码基于 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) 授权。

Spring、Spring Boot 和 Spring Cloud 是 [Pivotal Software, Inc.](https://pivotal.io/) 在美国和其他国家的注册商标。

## 快照构建
你可以通过在 `repositories` 中添加以下配置，从 GitHub 快照仓库获取快照构建版本：
```xml
<repository>
	<id>sba-snapshot</id>
	<name>Spring Boot Admin Snapshots</name>
	<url>https://maven.pkg.github.com/codecentric/spring-boot-admin</url>
	<snapshots>
		<enabled>true</enabled>
	</snapshots>
	<releases>
		<enabled>false</enabled>
	</releases>
</repository>
```

## 参与贡献
请参见 [CONTRIBUTING.md](CONTRIBUTING.md)。
