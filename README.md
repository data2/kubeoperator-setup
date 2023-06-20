# kubeoperator-setup

![image](https://github.com/data2/kubeoperator-setup/assets/13504729/6383a14d-3669-43aa-a8fe-62cdf6528e8e)

![image](https://github.com/data2/kubeoperator-setup/assets/13504729/223c4208-76b0-46c0-b589-b2b25c6b22bb)


## 离线安装

```
请自行下载 KubeOperator ​ ​最新版本的离线安装包​​，并复制到目标机器的 /tmp 目录下

cd /tmp
# 解压安装包
tar zxvf KubeOperator-release-v3.9.0-amd64.tar.gz
# arm64 的包名是 KubeOperator-release-v3.9.0-arm64.tar.gz
cd KubeOperator-release-v3.9.0
# 运行安装脚本
/bin/bash install.sh
# 等待安装脚本执行完成后，查看 KubeOperator 状态
koctl status

```

## 在线安装

## 使用

```
检查状态
安装完成后，检查服务状态。若有有异常，可以使用 koctl restart 命令进行重新启动
koctl status

登录
地址: http://<ko服务器_ip>:80
用户名: admin
密码: kubeoperator@admin123

帮助
koctl --help

```

## 离线升级

```
# 离线升级需要提前下载离线安装包，并解压到 KubeOperator 部署机
# 进入升级包目录
cd KubeOperator-release-v3.9.0
# 运行安装脚本
./koctl upgrade
# 查看 KubeOperator 状态
koctl status

```
