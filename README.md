# 补天SRC爬取

--L0nelyC1ty
--2022/8

## 环境

Python 3.10.6

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

***

python和包都用的截至22/8/7最新的

#### python下载地址

[Download Python | Python.org](https://www.python.org/downloads/)

#### 更新全部包

##### 更新pip

```python
python3 -m pip install --upgrade pip
```

##### 更新包

```python
# 列出全部包
pip list

# 安装更新全部包的第三方库
pip3 install pip-review

# 更新
pip-review --local --interactive
```
