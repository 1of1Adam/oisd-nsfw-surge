# oisd-nsfw-surge

这是将 oisd nsfw 域名列表转换为 Surge 可直接引用格式的仓库，方便通过网络链接加载最新的阻断规则。

## 文件
- `oisd_nsfw_domainswild2.list`: 依据 Surge `DOMAIN-SUFFIX` 语法生成的 42 万+ 域名规则。
- `index.html`: 简单网页入口，方便在浏览器中查看/下载列表文件。

## 使用方法
1. 直接引用 RAW 链接：
   ```
   https://raw.githubusercontent.com/1of1Adam/oisd-nsfw-surge/main/oisd_nsfw_domainswild2.list
   ```
2. GitHub Pages（若已启用）：
   ``
   https://1of1Adam.github.io/oisd-nsfw-surge/oisd_nsfw_domainswild2.list
   ``
3. Surge 配置示例：
   ```ini
   [Rule]
   RULE-SET,https://raw.githubusercontent.com/1of1Adam/oisd-nsfw-surge/main/oisd_nsfw_domainswild2.list,REJECT
   ```

可以根据需求定期替换文件内容（保持同名），再推送即可让引用链接获取最新规则。
