先去注册以下账户：

一个 GitHub 账号https://github.com

一个 Cloudflare账号https://dash.cloudflare.com

## 使用方法：Pages+Fork公开仓库
1. 登录自己的GitHub直接Fork本存储库[https://github.com/33995331/-BPB-Worker-Panel]

本存储库main主线默认为自动升级为最新版本，Fork后在（Actions行动）中打开工作流程就可以开启自动更新。

2. 到Cloudflare利用Pages+github搭建。

打开 Cloudflare → Workers & Pages → 点击创建 Pages；


选择 GitHub 仓库并连接 BPB 项目；

设置为生产环境构建并部署。

3. 再增加下面必要的变量。
 添加完变量后要重试部署
## 环境变量与说明（复制变量前将网页翻译切换到原文）
| 变量  | 用法 |
| :-------------: | :-------------: |
| **UUID**  | 必要；[在线生成](https://1024tools.com/uuid) ，用于生成 VLESS 节点配置 |
| **TR_PASS**  | 必要；密码，自行随意输入，用于生成 Trojan 节点配置  |
| **kv**  | 必要；KV命名空间  |

试问面板：/panel，部署成功后，在 url 后面增加/panel来进行访问面板，访问面板修改的密码将会保存在kv里。
