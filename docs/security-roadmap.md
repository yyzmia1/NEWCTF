# 网络安全 & CTF 学习路线：从零基础到实战，开启你的安全之旅

> **出品**：极客创新实验室 · 网络安全战队 著  
> **实战推荐平台**：[CTF 极客实战攻防靶场 (ctf.example.com)](https://ctf.example.com) *(建议先注册账号，随时动手实战)*  
> **在线导航站**：[NEWCTF 学习路线导航站 (index.html)](../index.html) | [全景技术思维导图 (mindmap.html)](../mindmap.html)

---

## 欢迎开启网络安全极客之旅

如果你在一众计算机技术方向里找到了网络安全组，那么你可能会疑惑：**网络安全到底是干啥的？**

是对着黑底绿字的屏幕敲几下回车，就能接管整栋大楼的电脑；是戴上连帽衫在键盘上十指残影，就能三秒钟攻破层层防火墙；还是点开满屏看不懂的闪烁弹窗，就能在谈笑间掌控全城电网、调取街头每一处监控？不妨先看看这两个视频直观感受一下：

- 🎬 **科普启蒙**：[【一个视频，从0到1带你了解网络安全！】(B站视频)](https://www.bilibili.com/video/BV1Jgf6YvE8e)
- 🚩 **夺旗赛入门**：[【CTF入门教学】大学生必看！CTF 夺旗赛入门秘籍(B站视频)](https://www.bilibili.com/video/BV1th411z7sn/)

在学习起步阶段，带大家接触的切入点主要是 **CTF（Capture The Flag，夺旗赛）**——也就是通过解题闯关的方式，在合法的竞赛平台或本地靶场里分析漏洞、找出隐藏的“旗帜”（通常是一串形如 `flag{...}` 的字符）。

但请记住：**CTF 只是网络安全学习中的重要一环和最佳练兵场，而不是全部。** 我们的完整路线是从基础代码起步，借 CTF 打磨漏洞原理，最终走向更广阔的真实世界安全实战。

---

## 总体路线与核心学习思路

完整学习路线分为四个阶段：**代码与环境起步** ➔ **CTF 五大赛道专项攻防** ➔ **攻防演练与工程实战** ➔ **前沿安全研究与 AI 安全**。

> **学习节奏建议**：  
> **不必等学完所有基础再开始做题**，也不需要一开始就掌握全部方向。先上手体验入门题，遇到知识缺口时，再回到相应资料补齐即可。

---

## 第一阶段：最小化起步准备（代码与环境）

网络安全的学习离不开代码底子：前期写自动化解题脚本（Exp）、算密码题，主要靠 **Python**；如果往后想研究程序逆向或二进制漏洞，则需要看懂 **C 语言** 代码。工具也不必第一天就全装齐，先配好 Python、虚拟机和浏览器开发者工具（F12）即可开干：

### 1. Python 语言（自动化脚本必备）
- **核心要求**：掌握字符串、列表、字典、函数和文件读写，能读懂并修改简单脚本即可。
- **推荐资源**：
  - [3小时超快速入门Python | 动画教学 (B站视频)](https://www.bilibili.com/video/BV1bGMnz5EJs)
  - [菜鸟教程：Python 3 教程](https://www.runoob.com/python3/python3-tutorial.html)
  - [Python 官方中文文档 (3.12)](https://docs.python.org/zh-cn/3/tutorial/index.html)

### 2. C 语言基础（二进制与底层逻辑）
- **核心要求**：重点理解指针、内存分配与数组，为后续逆向工程（Reverse）和二进制漏洞挖掘（Pwn）打基础。
- **推荐资源**：
  - [【郝斌】C语言自学视频教程 (B站优质)](https://www.bilibili.com/video/BV1f5X5Y5EYH/)
  - [菜鸟教程：C 语言教程](https://www.runoob.com/cprogramming/c-tutorial.html)
  - [C 语言经典实例 100 例](https://www.runoob.com/cprogramming/c-examples.html)

### 3. Linux 基础操作与终端命令
- **核心要求**：掌握基础命令（`cd`、`ls`、`grep`、`chmod`、`ssh`），学会使用 Linux 命令行交互。
- **推荐靶场与教程**：
  - [OverTheWire: Bandit 闯关游戏 (最富趣味的 Linux 命令行实战)](https://overthewire.org/wargames/bandit/)
  - [【狂神说Java】Linux最通俗易懂教程 (B站视频)](https://www.bilibili.com/video/BV18t411373T/)

### 4. Git 版本控制与工程协作
- **核心要求**：掌握 `git clone`、`git commit`、`git push`、分支管理与 GitHub/Gitee 协作规范。
- **推荐资源**：[Git 官方中文手册 Pro Git](https://git-scm.com/book/zh/v2)

---

## 第二阶段：CTF 五大核心赛道专项攻防

### 🌐 Web 安全（网站漏洞攻防）
- **方向介绍**：挖掘与利用 Web 应用中的各类安全隐患，包括 SQL 注入、XSS 跨站脚本、文件上传、SSRF、命令执行与反序列化。
- **实战靶场**：
  - [PortSwigger Web Security Academy (全球顶级官方免费靶场)](https://portswigger.net/web-security)
  - [CTFHub 技能树 (中文结构化入门)](https://www.ctfhub.com/)
  - [CTF.show 题库 (国内权威)](https://ctf.show/)

### 🔐 Crypto（密码学攻防）
- **方向介绍**：研究经典密码体制、对称密码（AES/DES）、非对称密码（RSA/ECC）、哈希算法抗碰撞性以及数学原理。
- **实战资源**：
  - [CryptoHack (全球最好玩的密码学闯关平台)](https://www.cryptohack.org/challenges/introduction/)
  - [CTF-Wiki 密码学模块](https://ctf-wiki.org/crypto/classical/summary/)

### 🔍 Reverse（逆向工程）
- **方向介绍**：将编译后的二进制可执行程序“拆开”，通过静态反汇编（IDA Pro / Ghidra）与动态调试（x64dbg / GDB）还原关键逻辑与破解算法。
- **核心工具**：IDA Pro、Ghidra、010 Editor、x64dbg
- **实战资源**：[CTF-Wiki 逆向模块](https://ctf-wiki.org/reverse/summary/)

### 💣 Pwn（二进制漏洞挖掘与利用）
- **方向介绍**：通过缓冲区溢出、格式化字符串漏洞、ROP（返回导向编程）或堆漏洞利用，绕过系统防护机制（DEP/NX、ASLR、Canary），最终获取服务器 Root Shell。
- **实战资源**：
  - [CTF-Wiki Pwn 模块](https://ctf-wiki.org/pwn/linux/user-mode/stackoverflow/x86/stack-intro/)
  - [Pwntools 官方文档](https://docs.pwntools.com/)

### 🧩 Misc（安全杂项与数字取证）
- **方向介绍**：涵盖隐写术（图片/音频隐写）、流量分析（Wireshark 抓包缉凶）、磁盘内存取证（Volatility）、工控安全及各种奇妙逻辑解谜。
- **核心工具**：Wireshark、Volatility、CyberChef、Audacity

---

## 第三阶段：攻防演练与工程化进阶

- **AWD 攻防对抗 (Attack With Defense)**：即时修补自身服务漏洞，编写自动化攻击脚本，实施攻防双向博弈。
- **内网渗透与域控攻防**：红队实战、横向移动、权限提升、内网穿透与隧道构建。
- **漏洞披露与安全众测**：在国家信息安全漏洞共享平台（CNVD/CNNVD）及各大企业 SRC 平台提交合规漏洞。

---

## 第四阶段：前沿安全研究与 AI 安全

- **LLM/AI 安全**：探索针对大语言模型的越狱提示词注入（Prompt Injection）、训练数据投毒、大模型 API 供应链漏洞等前沿议题。
- **内核与移动安全**：Linux/Windows 内核提权、Android/iOS 逆向、Frida 动态 Hook。

---

## 极客守则与红线规范

1. **合法合规第一**：所有技术实践必须在合法授权靶场或本地虚拟机环境中运行。严禁未经授权对公网资产进行扫描、渗透或攻击。
2. **拒绝脚本小子**：不仅要会用工具，更要掌握漏洞成因与修复方案。
3. **开源共享精神**：坚持编写复盘 Writeup，分享学习成果，与技术社区共同成长。
