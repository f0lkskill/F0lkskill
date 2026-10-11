<div align="center">

# 👋 Hi, I'm f0lkskill

**桌面端轻量级程序开发者 · Python 全栈 · 原生前端信徒**

[![GitHub followers](https://img.shields.io/github/followers/f0lkskill?label=Followers&style=social)](https://github.com/f0lkskill)
[![GitHub Stars](https://img.shields.io/github/stars/f0lkskill/FaustLauncher?label=Stars&style=social)](https://github.com/f0lkskill/FaustLauncher)

</div>

---

## 🧑‍💻 关于我

你好，我只有两岁！😄

我专注于 **桌面端与轻量级 Web 程序** 的开发，主技术栈是 **Python 后端 + 原生 HTML/JS 前端**。

我的技术信条很简单：

> **无框架、无数据库、无构建步骤。能用标准库解决的事，绝不引入第三方依赖。**

这不是偷懒，而是一种取舍 —— 我宁愿花时间把一件事做透，也不愿把项目堆成依赖的迷宫。

---

## 🛠️ 技术栈

Python    ████████████████████  标准库 · Bottle · requests · Pillow · PyInstaller
桌面应用  ████████████████████  pywebview · WebView2 · 多进程窗口模型
前端      ████████████████░░░░  原生 HTML/CSS/JS · CSS 变量 · 无框架架构
Web 后端  ████████████████░░░░  WSGI · 原子写 · HMAC 签名 · 会话与权限
逆向工程  ████████████████░░░░  capstone · pefile · pythonnet · UnityPy
工程化    ████████████████░░░░  自动更新 · 资源包分发 · 多源回退 · 诊断工具

---

## 🚀 项目

### 🖥️ FaustLauncher — 桌面端

《边狱巴士》一体化启动器，为玩家提供汉化、美化、Mod 管理的**一键启动流水线**。

这个项目里我做了这些事：

- **桌面架构** —— 用 pywebview + 原生前端替代 Electron，无框架依赖，冷启动快、内存占用低；主窗口与子进程窗口分离，绕开 pywebview 主线程互斥限制
- **系统层操作** —— 符号链接搬运、文件原子替换、更新失败回滚、Windows Script Host 脚本，全部亲手处理
- **逆向工程** —— 读 PE 结构、解析 Unity 资源、做内存 Hook 与偏移索引，把底层能力封装成用户的一次点击
- **完整分发** —— PyInstaller 打包、独立资源包体系、多源回退与缓存降级，一个人跑通从构建到更新的全链路

### 🌐 FaustLauncherWeb — 云端后端

上述启动器的云端后端与官网，目前承载 **600+ 用户、40+ Mod、11 万+ 次接口调用**。

这个项目里我做了这些事：

- **无数据库后端** —— 用纯文本笔记做存储，按 key 寻址，换机器只需拷 data/ 目录；没有 ORM、没有脚手架，Bottle 单文件跑完整个 WSGI 应用
- **并发安全设计** —— 所有写入走「临时文件 + os.replace」原子替换，避免截断写与并发读的竞态；服务端锁内「读整表 → 只改一行 → 写回」，客户端永不提交整张表
- **标准库级加密** —— 用 hmac / hashlib / base64 实现登录 Cookie 签名与用户主页令牌加密（CTR 流加密 + 截断 HMAC 校验），零第三方加密依赖
- **权限与隐私** —— 账号即 ID、无密码登录、管理员双通道识别、用户 ID 默认打码，本人或管理员才拿得到真实 ID
- **部署自动化** —— 自写增量同步脚本，走官方 API 比对差异、上传、重载，支持 dry-run 与远程清理

> 两个项目共享同一套哲学：**把复杂度留给自己，把简单留给用户。**

---

## 📊 GitHub 数据

<div align="center">

![f0lkskill's GitHub stats](https://github-readme-stats.vercel.app/api?username=f0lkskill&show_icons=true&theme=radical&hide_border=true&count_private=true)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=f0lkskill&layout=compact&theme=radical&hide_border=true)

</div>

---

## 💖 支持我

如果我的项目帮到了你，欢迎通过爱发电支持持续开发：

<div align="center">

[![爱发电](https://img.shields.io/badge/爱发电-赞助支持-ff69b4?style=for-the-badge)](https://afdian.com/a/f0lkskill)

</div>

---

<div align="center">

**感谢来访，欢迎 Star ⭐ 和关注！**

<sub>Built with ❤️ for Limbus Company players.</sub>

</div>
