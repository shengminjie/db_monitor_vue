## 项目介绍

> 基于 iview-admin 2.5.0


## 运行

```bush
1. 下载项目源码
git clone https://github.com/gumengkai/db_monitor_vue

2. 修改后端API连接地址
src/config/index.js
baseUrl:
    dev: 测试
    pro: 线上
示例API地址：47.100.119.84:43278

补充：
1、安装yarn：
curl -o- -L https://yarnpkg.com/install.sh | bash -s -- --nightly
环境变量注意最后提示，如果路径不对需要自己配置
2、运行还是需要，Yarn requires Node.js 4.0 or higher to be installed
官网下载稳定版https://nodejs.org/en/download/
tar xf node-v12.18.1-linux-x64.tar.xz                                   // 解压
cd node-v12.18.1-linux-x64                                              // 进入解压目录
老规矩先备份，养成修改重要文件之前先备份的好习惯。
cp /etc/profile /etc/profile.bak
然后 vim /etc/profile，在最下面添加 export PATH=$PATH: 后面跟上 node 下 bin 目录的路径
export PATH=$PATH:/root/node-v12.18.1-linux-x64/bin
立即生效
source /etc/profile
[root@localhost ~]# node -v
v12.18.1



3. 安装依赖包
yarn install

4. 开发环境运行
yarn run dev
```

## DEMO

> http://122.51.204.250:8080/

> 账户 admin 密码 111111

![demo1](src/demo/demo1.jpg)
![demo2](src/demo/demo2.jpg)

## 编译

> dist

```bush
yarn build
```

将dist文件夹部署到nginx即可
