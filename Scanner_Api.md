
## 0，全局定义

### API返回统一返回Json对象格式

- status (0或1，请求错误返回 0 ，请求成功返回 1)
- info （当请求失败时提示的信息）
- data 用户数据

### session处理

1. 登陆后后天作session处理
2. 每个API调用时都加上用户名和密码这两个参数


## 1，登录

### 参数

- 用户名
- 密码

### 返回

用户id

## 2，注册

### 参数

- 用户名
- 密码
- 地址
- 手机号

### 返回

用户id

## 3，快递员用户生成快递订单

在手机填写一系列表单字段后点击生成订单，后台生成对应唯一的二维码（可以根据订单id生成）

### 参数

- 用户id
- 快递订单编号
- 寄件人姓名
- 寄件人地址
- 寄件人手机号
- 收件人姓名
- 收件人地址
- 收件人手机号

### 返回

- 订单id

## 4，手机扫描某个快递订单二维码

通过扫描订单的快递员信息（用户名，地址，扫描时间）为快递添加物流信息

### 参数

- 用户id
- 订单id

### 返回

- 无

## 5，获取快递订单详情

### 参数

- 订单id

### 返回

- 发货快递员
- 订单生成时间
- 订单编号
- 寄件人姓名
- 寄件人地址
- 寄件人手机号
- 收件人姓名
- 收件人地址
- 收件人手机号
- 物流信息
- 二维码图片url

## 6，获取某个快递员生成的订单列表

### 参数

- 用户id

### 返回

- array【订单id，订单编号，订单生成时间】



