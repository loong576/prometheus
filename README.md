# Prometheus+Grafana+钉钉搭建监控告警系统
**环境说明：**

 
| 主机名 | Docker版本 | Prometheus版本 | Node exporter版本  | cAdvisor版本 | Grafana版本 | ip地址 |
|:------:   |:------:|:------:|:------:|:------:|:------:|:------:|
| docker01 | 18.09.2 | 2.9.2 | 0.18.0 | v0.32.0 | v6.1.6 | 172.27.9.71 |
| docker02 | 18.09.2 | / | 0.18.0 | v0.32.0 | /| 172.27.9.75 |


<br>
 &emsp;  &emsp; Prometheus是一套开源的系统监控报警框架，提供了监控数据搜集、存储、处理、可视化和告警一套完整的解决方案，该项目于2012年在SoundCloud上创建，拥有非常活跃的开发人员和用户社区，许多公司和组织都采用了Prometheus。作为一个独立的开源项目，Prometheus于2016年正式加入Cloud Native Computing Foundation，成为受欢迎度仅次于Kubernetes的项目。
程序编写环境：

**文章目录：**
# 一、Prometheus简介
# 二、Prometheus架构
# 三、Prometheus搭建
## 1. 环境说明
## 2. 监控主机部署 
### 2.1 docker-compose.yml配置
### 2.2 运行docker-compose
### 2.3 查看Node Exporter监控数据
### 2.4 查看cAdvisor监控数据
## 3. 监控服务器部署
### 3.1 prometheus.yml配置
### 3.2 docker-compose.yml配置
### 3.3 运行docker-compose
### 3.4 查看Prometheus监控数据
#### 3.4.1 配置文件查看
#### 3.4.2 监控信息查看
#### 3.4.3 查看指定监控项
# 四、Grafana配置 
## 1. 登陆grafana
## 2. 添加DataSource
## 3. Dashboards配置
### 3.1 下载Dashboards
### 3.2 导入 Dashboards
## 4. Grafana监控展示
### 4.1 容器监控展示
### 4.2 host监控展示
# 五、钉钉告警配置
## 1. 钉钉添加机器人
## 2. Grafana新增告警项
## 3. 新增告警项
### 3.1 编辑Memory Usage
### 3.2 创建Alert
### 3.3 Alert配置
### 3.4 验证告警配置
### 3.5 保存告警配置
### 3.6 告警信息查看

<br>
<br>
**详细搭建过程及测试：**
<br>
https://blog.51cto.com/3241766/2394283
