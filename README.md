# 徐塬富 · Yuanfu Xu

金融硕士，现在在做 Agent 运行时的底层控制。不是科班出身，所以更怕「这东西是什么时候悄悄坏掉的」。

**一句话**：给 agent 完全权限是危险的，只给它一个沙箱又憋屈。我想在中间造一个可调的管家——权限给够，但每一笔都记账。

## 在做什么

| 项目 | 它解决什么 |
|---|---|
| [dsh-confirm-gate](https://github.com/SteelUnion/dsh-confirm-gate) | 控制面。按轮数持久化操作，到额度先提醒、再要求停下、最后才问人。沙箱足以自保的模式下它保持沉默。 |
| [dsh-softsensor-hub](https://github.com/SteelUnion/dsh-softsensor-hub) | 感知面。统一收系统告警、天气、邮件、行情，判轻重再决定叫不叫醒你。四个采集器跑在插件进程里，793 项测试。它自己不动手。 |
| [dsh-wechat-queue](https://github.com/SteelUnion/dsh-wechat-queue) | 输入通道。微信消息先落盘再处理，严格串行，重启不丢。 |
| [dsh-plugin-manual](https://github.com/SteelUnion/dsh-plugin-manual) | 八册手记：通用四册（命令、网络、调试）+ DSH 内核四册（钩子、终态、注入门、发版）。踩过的坑都写进去了。 |
| [quant-toolkit](https://github.com/SteelUnion/quant-toolkit) | 一份能自己重建的 A 股数据库。5,600+ 标的，单个 SQLite，增量刷新。 |
| [exam-adb-pipeline](https://github.com/SteelUnion/exam-adb-pipeline) | 给一个不肯开接口的 App 装上眼睛和手。ADB + 节点树 + 手势 + OCR。 |

前两个已收录进 [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin)。

## 几条我在意的

- 没有终态的流程等于没有流程。「卡住」和「在干活」从外面看是一样的。
- 路径隔离管的是「写到哪」，不管「写多少」。四十次都合法的写入，照样能重写一个项目。
- 没有审计的拦截，事后说不清到底拦了什么。

> 刹车不是墙。墙只告诉你不能走，刹车让你知道自己开多快。

## 联系

哈尔滨工业大学（M.Sc. Finance）· 上海 · xuyuanfu1997@163.com
