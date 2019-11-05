# 如下操作在linux上操作总结
-----------------------------
## 1.git add filename 
     本地仓库添加文件
## 2.git commtit -F "comments"
     提交文件，并备注信息
## 3.用awk 提取提交的信息：
###  3.1 git log查看提交的信息
     NR---行 $后面跟数字表示列号
     git log | awk 'NR==1{print $1}'输出git log 里面第一行第一列的字段
##   3.2 自定义函数提取git log里面的信息

```shell
git log | awk '
{myfun();} 
function myfun(){
自定義內容
}
'
```
## 4.列出所有分支
     git branch -a
## 5.创建test分支
     git branch test
## 6.切换到test分支
     git checkout test
