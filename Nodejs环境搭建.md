### Nodejs环境搭建

Node Version Manager - POSIX-compliant bash script to manage multiple active node.js versions

### 安装

安装命令

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

配置环境变量及补全

```shell
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
```

### 使用

```shell
# 安装最新版本的nodejs
nvim install node
# 指定版本
nvm install 14.7.0
# 列出可选择的nodejs版本
nvm ls-remote
# 运行node
nvm use node
# 运行并指定版本
nvm run node --version 

```

