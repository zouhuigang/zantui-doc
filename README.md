# zantui-doc
Doc of iView


### 提交

创建分支,需要将(dist和dist/*)从.gitignore删除掉:

	git branch gh-pages
	git add -A
	git commit -m "..."
	git push origin master
    git subtree push  --prefix=dist  origin gh-pages



### zantui

	https://github.com/zantui/zantui-doc.git


### 问题汇总


Q:

	Error: Cannot find module 'yargs'


A:

	删除node_modules，重新安装


Q:

	vue-router报错：RangeError: Maximum call stack size exceeded，

A:

	