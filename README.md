# Introduction

MySQL-piper|MySQL管家, 是一个开源的MySQL一站式运维&审计&在线执行管理工具, 包含但不限于有如下功能及特性:

- 本质是一个proxy
    - 既是mysql server也是mysql client,本质是一个proxy
    - 用mysql client连接上来操作:
        - 配置后端server的帐号信息,查看命令:show servers;
        - 查看系统帮助:show helps;
- 带有审计功能
    - 使用"管道+server name"直接操作后端服务器,如: select version() => db1;
    - 自动记录操作者所有记录,生产数据查询脱敏处理
- 也有审核功能
    - 插件式审核功能,可根据"语法树"轻松定制自己的"军规"
    - 具有proxy功能,配置到系统中,可以直接收集所有的待审核语句
    - 批量生成审核报告
- 还有可选插件
    - 集成soar,在线SQL优化建议
    - 集成online ddl功能,增加定时执行功能
- 集成WebUI,更方便操作

### 典型应用场景:
- 统一管理生产环境MySQL帐号
- 集中管理开发者和DBA操作帐号权限
- 审计工单管理
- SQL规范自动审核
- SQL优化建议,集成soar实现


### 快速体验功能
[功能预览](Chapter1/功能预览.md)