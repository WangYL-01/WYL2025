# 使用指南

>1. 安装VS Code

>2. 安装python环境

>3. 创建虚拟环境：python -m venv .venv

>4. 权限获得：Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

>5. 激活虚拟环境：./.venv/Scripts/activate (Windows)\
                 source.venv/bin/activate (Linux)

>6. 安装jupyter-book：pip install jupyter-book

>7. 创建书：jupter-book create test 或者 jb creat test

>8. jb build .（在已有文档基础上修改内容直接 jb build . ）与jb clean . （一般只在目录（章节增删），配置文件有改动的时候）的使用

>9. 每次更新完记得保存(Ctrl+S)

>10. 本地与github关联以后，关键步骤
```
 > jb build . (本地网页更新，方便自己检查)
 > git add .  
 > git commit -m "comments(此参数按自己需求来写)" 
 > git push origin main  （push 到github以后，github会基于新的源文件生成新网页，即使你本地没有 jb build . 也没关系）
 > git pull （把网站上的最新内容同步下来）
```
