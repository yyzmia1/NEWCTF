# NEWCTF | 网络安全 & CTF 极客全景学习路线与实战导航系统

> 🛡️ **代码即武器，安全即使命。**  
> 一套从零基础起步、借 CTF 竞赛打磨底层原理、最终进阶至真实网络安全攻防与前沿 AI 安全的现代化开源知识系统。

---

## 🌟 项目亮点

- **现代化工程美学**：采用国际权威文档设计规范（纯净白/石板灰高保真排版），响应式自适应移动端与桌面端。
- **四大递进式学习阶段**：
  1. **代码与环境起步**：Python 自动化脚本、C 语言底层指针、Linux 核心操作与 Git 协作。
  2. **CTF 五大赛道专项攻防**：Web 渗透、Crypto 密码学、Reverse 逆向工程、Pwn 二进制漏洞、Misc 杂项取证。
  3. **攻防对抗与工程实战**：AWD 实时攻防对抗、企业内网渗透、合规漏洞挖掘与 SRC 众测。
  4. **前沿安全研究**：LLM 大模型越狱与提示词安全、内核提权与移动终端安全。
- **全景思维导图集成**：内置独立的 `mindmap.html` 交互式技术全景图谱，支持缩放、分类筛选与深度溯源。
- **离线文档中心**：提供完整的 Markdown 及 Word (`.docx`) 格式配套路线指引。

---

## 📂 项目结构

```plaintext
newctf/
├── assets/                       # 12 大核心赛道与技术背景图谱资源
│   ├── bg-*.png                  # 赛道技术主题图
│   └── trans_bg-*.png            # 水印与半透明卡片图层
├── docs/                         # 离线详细指引与知识库
│   ├── security-roadmap.md       # 学习路线全景 Markdown 文档
│   ├── security-roadmap.docx     # 学习路线 Word 文档
│   └── ctf-guide.md              # CTF 极客启航与五大赛道深度技术指南
├── index.html                    # 核心学习路线导航门户（主入口）
├── 1.html                        # 路线门户别名（兼容旧引用）
├── mindmap.html                  # 网络安全技术全景思维导图
├── .gitignore                    # Git 忽略配置
├── LICENSE                       # MIT 开源许可证
└── README.md                     # 项目说明文档
```

---

## 🚀 快速上手

### 本地直接浏览
本系统为纯静态无依赖架构，无需安装 Node.js 或构建工具：
1. 克隆本仓库到本地：
   ```bash
   git clone https://gitee.com/yyzmiao/newctf.git
   cd newctf
   ```
2. 双击直接在浏览器中打开 `index.html` 即可开始学习体验。
3. 点击顶栏导航可无缝跳转到 `mindmap.html` 查看技术全景思维导图，或进入 `docs/` 查阅路线文稿。

### 静态托管部署
本项目支持一键部署至各类静态托管服务：
- **Gitee Pages** / **GitHub Pages**：在仓库设置中启用 Pages，以根目录作为发布源即可。
- **Nginx / Caddy**：将仓库目录指向 Web 静态站点根目录。

---

## 🎯 核心赛道概览

| 赛道 / 方向 | 核心知识点 | 推荐入门工具 / 靶场 |
| :--- | :--- | :--- |
| **🌐 Web 安全** | SQL 注入、XSS、SSRF、文件上传、反序列化、SSTI | Burp Suite、PortSwigger Academy、CTFHub |
| **🔐 Crypto 密码学** | 古典密码、RSA 数论、ECC 椭圆曲线、AES/DES 对称加密 | CyberChef、SageMath、CryptoHack |
| **🔍 Reverse 逆向** | x86/x64 汇编、ELF/PE 文件结构、反反调试、花指令 | IDA Pro、Ghidra、x64dbg、010 Editor |
| **💣 Pwn 二进制漏洞** | 栈溢出、ROP 链、格式化字符串、堆利用（Fastbin/Unsorted） | Pwntools、Pwndbg、Checksec、ROPGadget |
| **🧩 Misc 杂项取证** | 流量分析（PCAP）、内存取证、文件隐写、音频隐写 | Wireshark、Volatility、Audacity |

---

## ⚠️ 免责声明与安全守则

1. **合法授权原则**：本项目所列举的技术路线、攻防案例与工具资料仅供网络安全技术爱好者、在校高校学生及白帽子研究人员学习研究使用。
2. **严禁非法攻击**：任何个人或组织不得利用本项目提供的资源对未获书面授权的真实互联网资产进行渗透测试或未授权探测。
3. **法律红线**：请严格遵守《中华人民共和国网络安全法》、《中华人民共和国数据安全法》及相关法律法规。

---

## 📄 许可证

本项目采用 [MIT License](LICENSE) 开源许可证。
