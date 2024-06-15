# 广州理工学院 课表脚本

## 用途

获取教务系统的课表数据

## 使用步骤

1. 下载仓库
2. 安装Python3
3. 进入文件夹，打开命令行
4. 安装依赖
   ```pip install -r requirements.txt```
5. 填写账号密码
```python
    username = ''
    password = ''
```
6. 例如
```python
    username = '学号'
    password = '密码'
```
7. 输入自己数据库database
```mysql
conn = pymysql.connect(host='127.0.0.1', user='root', password='root', database='', charset='utf8mb4')
```
8. 输入表名，示例表名是kebiao
```mysql
sql = '''insert into kebiao(name,teacher,room,day,attend,nums,enums) values (%s,%s,%s,%s,%s,%s,%s) ;
```
## 最后

1. progress.py和progress.bat在同一目录
2. 双击执行progress.bat文件
