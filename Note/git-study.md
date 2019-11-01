# 如下操作在linux上操作總結
-----------------------------
## git add filename 
### 向本地倉庫添加文件
## git commtit -F "comments"
### 提交文件，並添加備註信息
## 用awk 提取提交的信息：
### git log查看提交的信息
### git log | awk '{print ...}'  輸出語法
### NR---行 $後面跟數字表示列
### git log | awk 'NR==1{print $1}'輸出git log 裏面第一行第一列的字段
## 自定義函數提取git log 裏面的信息 
### 
```shell
git log | awk '
{myfun();} 
function myfun(){
自定義內容
}
'
```
