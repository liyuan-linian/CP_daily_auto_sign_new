# 南京工程学院体温自动打卡V3.0Beta板

## 正在开发测试中，不保证可用

## 免责声明
本项目仅供学习与研究交流使用，请勿用于非法和商业用途  
另外鄙视一下利用信息差牟利的同学  

## Feature
- 通过教务网登录进行提问打卡签到，签到时间为每天7点10分和12点10分
- 需要手动打卡过一次后（即有打卡记录），该项目才能正常运行
- 通过配置文件configure.json进行配置，每次配置无需重启服务
- 打卡后会将打卡结果通过qq邮箱发送，需要自己配置

## 签到配置说明
在configure.json下的students字段配置账号密码  
配置示例见configure.json  
> name字段表示姓名，方便看到用户是否签到成功  
> account字段为教务网账号  
> password字段为教务网密码  

## 邮箱配置说明
将打卡结果发送到邮箱中，方便查看代码是否正常运行  
可以选择是否启动如果不启动则不需要配置  
> need_send表示是否需要发送到邮箱,默认不发送，需要发送时值为True，不需要时值为False  
> sender字段表示发送者的邮箱，填写自己的qq邮箱即可   
> token字段表示你qq邮箱的token，获取方式看[这里](https://www.cnblogs.com/Alear/p/11594932.html)  
> receivers表示接收者的邮箱，可以和发送者邮箱相同，即允许自己发给自己

## 使用说明
python版本3.7  
命令行执行以下代码
```shell
pip install -r requirements.txt    
python manage.py  
```

##### 感谢水鱼实验室@licsber提供的技术支持