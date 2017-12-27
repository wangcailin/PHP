# PHP
PHP常用技能

## 消息队列
> 应用场景 秒杀 抢购 发送消息 发送卡券

 - Redis List
 - RabbitMQ
 
## 生成二维码
 - QR Code
 
## 即时通信
> 应用场景 客服 聊天 监控实时监控数据 群发
 - MeepoPS
 - workerman
 
## 抽象画图
> 应用场景 数据统计 性能统计
 - JpGraph


# 安装扩展

#### mcrypt扩展
yum install libmcrypt libmcrypt-devel php-mcrypt mhash

# php性能优化

> 避免使用魔法函数如__get()
> 尽量使用自带函数完成
> 自带函数功能一致的情况下性能不同
> 禁用错误抑制符@
> 合理使用内存,及时unset()释放不使用的内存(unset有释放不掉的内存)
