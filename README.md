# openidentityplatform-openam-v16.0.5 - 漏洞总览

| # | CVE | 端点 | 漏洞类型 | 状态 |
|---|---|---|---|---|
| 1 | CVE-2026-41573 | `GET /openam/json/users?_queryId=` | LDAP 注入（用户枚举/盲注） | VULNERABLE |
| 2 | CVE-2026-33439 | `GET /openam/base/*` 等 JATO 路径（`jato.clientSession`） | 不安全的 Java 反序列化 / RCE | CODE_AUDIT |
| 3 | CVE-2026-44202 | `POST /openam/sessionservice` | SSRF（会话通知回调） | CODE_AUDIT |
| 4 | CVE-2026-44203 | `GET /openam/oauth2/authorize`（`response_mode=form_post`） | 反射型 XSS | CODE_AUDIT |
| 5 | CVE-2026-44793 | `GET /openam/saml2/SSO/POST`（autosubmitaccessrights.jsp） | 反射型 XSS | CODE_AUDIT |
| 6 | CVE-2026-45048 | `GET /openam/json/sessions?_queryFilter=` | 越权 / 信息泄露 | CODE_AUDIT |
| 7 | CVE-2026-45049 | `GET /openam/cdcservlet` | 会话劫持 / 信息泄露 | CODE_AUDIT |
| 8 | CVE-2026-45051 | 全局配置 | 不安全的 Java 反序列化 / RCE | CODE_AUDIT |
| 9 | CVE-2026-45052 | `POST /Liberty/*`（SOAPReceiver / Discovery） | 认证绕过 / 越权写入 | CODE_AUDIT |
| 10 | CVE-2026-45794 | `POST /openam/json/push/sns/message` | 不安全的 Java 反序列化 | CODE_AUDIT |
| 11 | CVE-2026-46498 | `POST /openam/json/push/sns/message` | OAuth 授权令牌伪造 / 越权 | CODE_AUDIT |
| 12 | CVE-2026-46560 | 全局配置 | 认证绕过（RADIUS 欺骗） | CODE_AUDIT |
