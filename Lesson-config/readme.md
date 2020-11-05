# 2020.11.05

## 配置
1. go 换源
    go env -w GO111MODULE=on
    go env -w GOPROXY=https://goproxy.cn,direct

2. 配置 node 源
    npm config set registry https://registry.npm.taobao.org

3. VScode出现无法识别命令时，可能是权限不足，前往属性->兼容性->选择以管理员运行

4. git 配置
    - 远程连接   git config --global user.name "yourname"

                git config --global user.email "your_email@youremail.com"
    - 生成密钥   ssh-keygen -t rsa -C "your_email@youremail.com"
    - 验证密钥   ssh -T git@github.com
    - 连接仓库   git remote add origin https://github.com/yourName/repositoryname.git
    - 仓库pull   git pull origin master
    - 查看工作目录的状态  git status
    - 上传代码   git add <filename>
    - 提交备注   git commit -m "message"
    - push文件   git push origin master (若 push 不成功，可加 -f 进行强推操作)
    - 添加key    SSH新建公钥

## 安装
1. go 安装 以 zip安装，需要配置环型变量，以及 config 文件写入

2. mongodb 安装，创建 data 文件、mongo.log 文件、mongo.conf 文件，在mongo.conf文件中写入相应配置

3. node 安装，使用msi安装包

4. robo 3T(数据库可视化工具) 安装

5. 数据库初始化：mysqld --initialize --console

6. cmd 设置管理员权限 打开cmd所在位置 -> 属性 -> 快捷方式 -> 高级 ->以管理员打开
