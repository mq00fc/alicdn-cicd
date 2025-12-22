# SSL证书自动化管理

本项目使用 GitHub Actions 自动申请和部署 SSL 证书到阿里云 CDN。

## 最近运行状态

- **状态**: ❌ 失败
- **最后运行时间**: 2025-12-22 09:53:03 (北京时间)
- **运行ID**: 20419357385

## 功能说明

- 自动使用 acme.sh 申请 SSL 证书
- 支持多域名一次性申请
- 自动上传证书到阿里云 CDN
- 每月自动运行一次
- 支持手动触发

## 配置说明

需要在仓库的 Settings > Secrets 中配置以下变量：

- `ALI_KEY`: 阿里云 AccessKey ID
- `ALI_SECRET`: 阿里云 AccessKey Secret
- `CERT_DOMAINS`: 证书域名列表（空格或|分隔）
- `CDN_DOMAINS`: CDN域名列表（空格分隔）
- `ACME_EMAIL`: ACME 注册邮箱（可选）
- `WECHAT_WEBHOOK`: 企业微信通知webhook（可选）

---

*本 README 由 GitHub Actions 自动更新*
