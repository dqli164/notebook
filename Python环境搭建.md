## Python环境搭建

### pipenv

> https://github.com/pypa/pipenv

安装

```shell
brew install pipenv
```

查看是否安装成功

```shell
pipenv --version
```

添加命令补全

```shell
eval "$(_PIPENV_COMPLETE=zsh_source pipenv)"
```

### pyenv

>https://github.com/pyenv/pyenv

pyenv lets you easily switch between multiple versions of Python. It's simple, unobtrusive, and follows the UNIX tradition of single-purpose tools that do one thing well.

安装

```shell
brew install pyenv
```

添加环境变量

```shell
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
```

依赖管理文件==Pipile==

```toml
[[source]]
url = "https://pypi.org/simple"
verify_ssl = true
name = "pypi"

[packages]
Scrapy = ">=2.2.1"
pyperclip = ">=1.5.27"
python-dotenv = ">=0.7.1"
ratelimit = ">=1.4.1"
selenium = ">=4.4.3"
slacker = ">=0.9.60"
tldextract = ">=2.1.0"
pytest = ">=3.10.0"
requests-iap = ">=0.2.0"
python-helpscout-v2 = ">=1.0.1"
algoliasearch = ">=2.0,<3.0"
typesense = "==0.10.0"
python-keycloak-client = "==0.2.3"

[dev-packages]
pylint = ">=2.3.1"

[requires]
python_version = "3.10"
```

安装依赖

```shell
pipenv install
```

激活虚拟环境

```shell
# To activate this project's virtualenv, run pipenv shell.
# Alternatively, run a command inside the virtualenv with pipenv run.
pipenv shell
```

