# githup
# lesson1

# sh
kali 开启 SSH 服务
端口映射 ： win7 2222 => kali 22
SSH 软件登录 Kali 服务器
```
# 查看本地端口开启
netstat -natp

# 打开 ssh
sudo /etc/init.d/ssh start

# 检测一下 22端口是否开启
netstat -natp
```
1.kali 开启 SSH 服务器
2.VmWare 端口映射
3.Termius 添加 Host, 本地端口和第二步保持一致。
4.Termius SSH OK

```
### 开机启动
sudo systemctl enable ssh

### 启动ssh 服务 （运行一次）
sudo systemctl start ssh
```
# lesson3
编辑 /etc/apt/sources.list 文件, 在文件最前面添加以下条目：
```
deb https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
deb-src https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
```
更改完 sources.list 文件后运行
