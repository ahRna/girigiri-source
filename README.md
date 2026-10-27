# Animeko 数据源 · girigiri 愛動漫

用于 [Animeko](https://github.com/Him188/ani) 的第三方在线数据源订阅，收录 **girigiri愛動漫** 一条源。

> 本仓库只存放数据源解析配置（JSON），不存储、不托管任何视频文件。

---

## 订阅地址

把地址里的 `你的用户名` 和 `仓库名` 换成你自己的实际值：

```
https://raw.githubusercontent.com/你的用户名/仓库名/main/girigiri.json
```

GitHub 直连较慢时，在地址前加加速前缀，任选其一：

```
https://gh-proxy.com/raw.githubusercontent.com/你的用户名/仓库名/main/girigiri.json
https://ghfast.top/raw.githubusercontent.com/你的用户名/仓库名/main/girigiri.json
https://ghproxy.link/raw.githubusercontent.com/你的用户名/仓库名/main/girigiri.json
```

---

## 使用方法

1. 打开 Animeko → **设置** → **数据源管理** → **订阅**
2. 点 **+** 添加订阅，粘贴上面的订阅地址，确定
3. 下拉刷新订阅，列表中会出现 **girigiri愛動漫**，确认已启用
4. 打开番剧 → 剧集 → **选择数据源** → 选 **girigiri愛動漫** 及对应线路

> 注意：`girigiri.json` 是订阅文件，需在「订阅」里添加；不要用「导入数据源」去导入单个源配置。

---

## 数据源信息

| 项目 | 内容 |
| --- | --- |
| 名称 | girigiri愛動漫 |
| 源 ID | `girigiri-ai-dongman` |
| 站点 | [ani.girigirilove.com](https://ani.girigirilove.com) |
| 类型 | 在线源（`web-selector` v2） |
| 优先级 | T0 |
| 依赖 | 无，纯网页源，不依赖任何中间层或自建服务 |

### 内置策略

| 策略 | 取值 | 说明 |
| --- | --- | --- |
| 请求间隔 | 3 秒 | 降低对站点压力 |
| 搜索缓存 | 2 小时 | 重复搜索直接命中缓存 |
| 搜索关键词 | 仅取第一个词，剔除特殊字符 | 提高命中率 |
| 默认分辨率 | 1080P | |
| 默认字幕 | 简体中文 | |
| 视频请求头 | 附带 `Referer` | 站点防盗链所需 |

---

## 更新方式

同名文件覆盖上传并提交即可，**订阅地址保持不变**，Animeko 下拉刷新订阅即可生效。

GitHub 的 raw 链接有约 5 分钟 CDN 缓存，刚改完没变化属于正常现象；急用可在地址后加 `?v=2` 之类的参数绕过缓存。

---

## 仓库结构

```
.
├── README.md        本说明
└── girigiri.json    订阅文件（Animeko 订阅用这个）
```

---

## 免责声明

- 本仓库仅提供播放地址的解析规则，**不存储、不托管、不分发任何视频内容**。
- 所有内容均来自第三方站点，版权归原权利人所有。
- 请勿用于商业用途，下载后请于 24 小时内删除，仅供学习与技术交流。
- 使用本数据源产生的一切后果由使用者自行承担。

---

## 致谢

- [Animeko](https://github.com/Him188/ani) — 优秀的开源动漫播放器
- 数据源站点及其运营者
