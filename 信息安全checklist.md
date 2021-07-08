# 信息安全checklist

- 数据安全
- 传输安全
- 内容安全
  - https://console.cloud.tencent.com/cms/text/overview



- [x] 数据库
  - [ ] https://dev.mysql.com/doc/refman/8.0/en/security.html
  - [x] 账号分级管理
  - [x] 定期备份 mysqldump
  - [ ] 主从备份
- [ ] 服务器
  - [ ] 账号权限管理
  - [ ] 端口管理，仅开放80，443
  - [ ] ssh不允许密码登录
- [ ] 前端
  - [ ] js代码混淆加密
- [ ] 后端
  - [ ] 接口鉴权
  - [ ] 接口限流
  - [x] `local_settings.py` 存密钥信息
  - [ ] cookie安全策略
  - [ ] csrf防护
- [ ] 网关层
  - [ ] nginx限流策略
  - [ ] 封高频访问ip
- [ ] 腾讯云安全策略
  - [ ] CDN
  - [ ] 云服务器安全组配置
  - [ ] 云监控dashboard
