# 补天SRC爬取

--L0nelyC1ty
--2022/8

## 环境

我是Python 3.10.5

```python
pip install -r .\requirements.txt
```



## 获取cookie

+ 登录补天
+ F12
+ 网络(Network)
+ 右键复制cookie值
+ 粘贴到butian.py对应位置



## 运行

```python
python .\butian.py
```

### 运行方式--全部爬取

+ 获取总页数
+ 获取所有company_id
+ 获取所有URL
+ 执行完毕，文件保存当前目录butian.csv

### tips

获取失败原因可能有，某页厂商/域名为空，或者厂商填写不规范，不影响继续执行。

访问频率过快，server端会回复一段混淆处理过的JS代码让client端执行并返回执行结果，

故全部爬取耗时较长sleep(1)。
