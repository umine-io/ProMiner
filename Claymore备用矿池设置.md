## Claymore备用矿池设置
  Steps:
  
    1.在claymore目录下创建epools.txt配置文件（path: /home/umine/mining/claymore）
    
    2.每行可以设置一个矿池，每个矿池会尝试连接3次，如果矿池长时间没有发送任务或者拒绝太多次则自动断开连接（开头字符为;和#当前行会被忽略）
    
    3.设置完成后可以重启或者在claymore运行窗口按'r'，重新载入epools.txt配置
    
    [参考范例]
      POOL:backup-eth.f2pool.com:8008, WALLET:<wallet address>, PSW:x, ESM:0, ALLPOOLS:0
