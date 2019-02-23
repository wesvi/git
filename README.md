## Git安装使用

``` bash
git --version
```

### 配置个人信息

``` bash
git config --global user.name "yourname"
git config --global user.email "youremail@example.com"
```

### 生成SSH公钥

``` bash
ssh-keygen -t rsa -C "youremail@example.com"
```

测试

``` bash
ssh -T git@github.com
```

### 常用命令

```bash
git init
git add .
git commit -m "注释语句"
git remote add origin https://自己的仓库url地址
git pull origin master
git push -u origin master
git rm -r --cached X/X
```
