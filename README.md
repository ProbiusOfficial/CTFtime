## 关于

本项目为 [Hello-CTF](https://github.com/ProbiusOfficial/Hello-CTF) 的关联项目，这是一个基于 Issue模板 + GitHub Action 实现的自动化赛事信息更新。  

如需查看赛事信息，请前往：[https://hello-ctf.com/Event/](https://hello-ctf.com/Event/)

## 数据来源

国外赛事数据来源于 CTFtime RSS源 - https://ctftime.org

国内赛事由本项目收集维护，如需要添加赛事信息，请选择Issue中的[添加比赛模板](https://github.com/ProbiusOfficial/Hello-CTFtime/issues/new/choose).

如有疑问，请开空白issue，或者在 [赛事群](https://qm.qq.com/q/HxicU7ee2e) 中联系本人或者三哈.

## 日历订阅

自动化程序提供适用于 RFC 5545 标准的日历订阅链接，您可以通过下面的链接直接订阅：

国内赛事：https://raw.githubusercontent.com/ProbiusOfficial/Hello-CTFtime/main/calendar/CN.ics

国外赛事：https://raw.githubusercontent.com/ProbiusOfficial/Hello-CTFtime/main/calendar/Global.ics

## 获取数据

所有的比赛信息均以 json 格式呈现，您可以通过下面的链接直接获取json数据：

国内赛事:https://raw.githubusercontent.com/ProbiusOfficial/Hello-CTFtime/main/CN.json

```
状态说明:
"status": 0 # 报名未开始
"status": 1 # 报名进行中
"status": 2 # 报名已结束
"status": 3 # 比赛进行中
"status": 4 # 比赛已结束
```

国外赛事:https://raw.githubusercontent.com/ProbiusOfficial/Hello-CTFtime/main/Global.json

## 自动化流程

国外赛事每小时自动更新.

国内赛事：提交Issue → Bot提交Pr审核 → 管理员审核通过添加.

每小时根据 UTC+8 时间更新国内比赛状态.

国内超过60天的比赛会被归档在 /Achieve/CN_CTF.json 中.

## TODO

暂无，期待issue.
