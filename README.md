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

#### PHP语言级性能优化
 -  避免使用魔法函数如__get()
 -  尽量使用自带函数完成
 -  自带函数功能一致的情况下性能不同
 -  禁用错误抑制符@
 -  合理使用内存,及时unset()释放不使用的内存(unset有释放不掉的内存)
 -  合理使用正则
 -  避免在循环内做运算(循环内的计算式将会被重复计算)
 -  减少密集型业务(PHP不适合密集型运算的场景),适合衔接webserver与后端服务、UI呈现
 -  务必使用带引号的字符串做键值(PHP会将没有引号的键值作为常量,产生查找常量的开销)
 
#### PHP周边问题的优化
 -  减少文件类的操作(内存>>数据库>磁盘>网络)
 -  减少PHP发起的网络请求(设置超时时间,将串行请求并行化"使用curl_multi,使用swoole扩展")
