# 2026_HNCPC_CTF-AWDP

2026年湖南省大学生程序设计竞赛-网络攻防赛道的赛题及复现环境归档

# 题目索引

| 方向 | 题目 | 数量 |
| :--- | :--- | :---: |
| Misc | [童话故事](#童话故事) · [免费中转站](#免费中转站) | 2 |
| Web | [java upload](#java-upload) · [json](#json) | 2 |
| AWDP-Web | [funadmin](#funadmin) | 1 |
| Reverse | [NightGlass](#nightglass) | 1 |
| Pwn | [PatchNote](#patchnote) | 1 |
| AWDP-Pwn | [Clock](#clock) | 1 |
| Crypto | [MAYO](#mayo) | 1 |
| **合计** | | **9** |

# 题目描述
  
## Misc
### 童话故事
这里是童话爷爷故事屋，童话爷爷很会讲故事哦。据说童话爷爷藏着一个宝藏，想办法获取童话爷爷的宝藏！请提交dart{}，括号里的内容。
  
### 免费中转站
小张为了省钱，把AI编程助手Cline的API接入点配成了一个第三方“免费中转站”。最近他让Cline帮忙搭一个Flask登录功能，几天后安全团队发现他的机器有异常外连——疑似中转站对AI的响应做了中间人篡改，在AI回复里夹带了恶意命令，植入了木马。安全团队拿到了小张用户目录的取证快照(/home/xiaozhang/)，请分析这份快照，溯源分析恶意的木马。请注意完整的URL地址，需包含path路径。fag格式为dart{xxx}，请提交完整的dart{}内容
  
## Web
### java upload
CloudVault是一个轻量文件托管服务。请提交dart{xxx}，括号里的内容。
  
### json
一个登陆功能，使用了json解析登陆请求数据，背后会不会有什么安全隐患？请提交dart{xxx}，括号里的内容。
> Hint:  
>  1、关注fastjson版本  
> 2、注意java版本，想想fastjson今年有什么热门的漏洞  
  
## AWDP(Web)
### funadmin
FunAdmin基于thinkphp8.X+Layui2.11+requirejs开发权限(RBAC)管理框架。请提交dart{xxx)，括号里的内容。
> Hint:  
> 1、看看文件上传的函数  
> 2、关注有哪些进程有root权限  
  
## Reverse
### NightGlass
123123
  
## Pwn
### PatchNote
是一款还在测试中的离线笔记工具，支持导入文档、查看内容和复制指定片段。 Flag 格式：dart{xxx}，请提交dart{} ，括号里的内容。 （配置socks5代理后，访问 nc 192.0.100.2 9999）
  
## AWDP(Pwn)
### Clock
小明挖到了一个CVE漏洞，他说这个漏洞藏在一个不起眼的角落，你能找到这个漏洞并完成利用吗？（flag位置为/flag，本地调试时请设置GLIBC_TUNABLES环境变量为glibc.malloc.arena_max=1，Bash/sh/Zsh设置命令：export GLIBC_TUNABLES="glibc.malloc.arena_max=1"） （配置socks5代理后，访问 nc 192.0.100.2 9999.Flag 格式：dart{xxx}，请提交dart{} ，括号里的内容。）
> Hint:  
> 1、漏洞诱因是未对输入补0  
> 2、漏洞成因是strsep()会将字符串内的A字节替换为B字节，想一想这个功能是如何造成内存破坏的  
  
## Crypto
### MAYO
我们给固件签名认证换上了后量子算法——MAYO。GF(16)上的多变量二次方程组，量子计算机也算不动，管理员对这套登录系统很放心。不过说实话，这台签名硬件最近有点不稳定：它内部的关键向量偶尔会"毛刺"一两个坐标。运维不想停机检修，顺手把出错时的输出接到了一个调试接口上放了出来“反正你也不知道错在哪，看看也无妨。”。试试看能不能登录？请提交dat{}，括号里的内容。（配置socks5代理后访问 nc 192.0.100.2 40133）


