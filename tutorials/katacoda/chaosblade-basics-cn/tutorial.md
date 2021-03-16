# ChaosBlade 基础教程

## 查看执行结果
通过 `top` 命令查看 CPU 使用率
````console
CPU usage: 93.79% user, 6.20% sys, 0.0% idle
````

## 恢复实验
此时命令已经生效，停止混沌实验，执行：
````bashinline
blade destroy 7c1f7afc281482c8
````
返回以下结果，表示停止实验成功
````console
{"code":200,"success":true,"result":"command: cpu fullload --debug false --help false"}
````

## 查看恢复结果
再去观察 CPU 情况，CPU 负载已回到正常状态：
````console
CPU usage: 6.36% user, 4.74% sys, 88.88% idle 
````
一次 CPU 满载演练完成。
