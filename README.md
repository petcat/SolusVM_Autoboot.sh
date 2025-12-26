# SolusVM 自动开机脚本

很多小鸡都是使用SolusVM，很多小鸡配置很低，超售严重，关机掉线是会有的，但后台提供API，那就可以通过API远程查询小鸡状态，发现关机就去重启。   
 

通过 API 会返回小鸡状态：<status>success</status><statusmsg>online</statusmsg><vmstat>online</vmstat><hostname>hostname</hostname><ipaddress>xxx.xxx.xxx.x</ipaddress>   
如果 online 就路过，如果 offline 就自动远程重启。可以扔在 crontab 每天自动运行一次。保证每天在线啦。
