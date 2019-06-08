# 遇见Docker - NEUMSC动手实验室

![head](https://github.com/IvyB/Docker-hand-on-NEUMSC/raw/master/img/head.png)

满足你对 **操作简单**、**跨平台**、**易于部署**、**高性能** 的需求。

一键管理复杂应用？

应用快速迁移到新机器？

快速安装一个复杂程序？

随意瞎搞也不怕搞坏系统？

虚拟化环境性能接近宿主机?

上面👆这些都在**几秒钟**的时间内完成？

上面👆这些都只用**几行命令**就轻松完成？

**Docker 都可以搞定**

![](https://tzr-1251830633.cos.ap-beijing.myqcloud.com/wudi.jpg)



## 物理机 vs 虚拟机 vs 容器 有什么区别？？

- 从虚拟化原理角度思考
- 从程序进程运行角度思考

具体现场见 :D



## Docker vs Dockerfile vs Docker compose 名词解释

- Docker：容器程序、服务

- Dockerfile：容器使用的镜像

- image：启动容器使用的镜像，可由dockerfile编译得到

- container: 由镜像得到的容器，可直接启动

- docker-compose：一个简单好用的多个容器编排管理工具



## 今天玩什么

1. 秒秒钟启动 **Nginx**

2. 编写 **Dockerfile**，制作一个自定义镜像

3. 编写 **docker-compose** 管理多个容器组成的服务 (WordPress为例)
4. 分分钟启动 **WordPress**

5. 分分钟启动 **JavaWeb** 应用 (使用打好包的war文件)

6. 分分钟启动 **Hadoop** //待定

7. 分分钟启动部署一个运维监控系统 (**Prometheus**+**Grafana**) //待定



## 安装 Docker

经过测试 CentOS 7、Debian 9、Ubuntu 18.04 均可成功安装

```shell
curl -sSL https://get.daocloud.io/docker | sh  
```

配置加速镜像。去申请一个自己的加速地址，加速地址申请： https://cr.console.aliyun.com/?spm=a2c4e.11153959.blogcont29941.9.699b69d6JE3Sgg#/accelerator

```shell
sudo mkdir -p /etc/docker  
sudo vim /etc/docker/daemon.json  
```

```json
{
  "registry-mirrors":["https://xxxxxxxx.mirror.aliyuncs.com"]
}
```

启动服务

```shell
sudo systemctl daemon-reload  
sudo systemctl enable docker  
sudo systemctl restart docker  
```



## ssh 连接演示机

我准备了一个性能不咋地的虚拟机，参加活动的小伙伴可以ssh登录。虚拟机已经安装好了 Docker 并拉取了几个常用的 Docker image



## Docker 简单命令





## Docker vs Docker Compose



