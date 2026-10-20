[English](README.md) | **简体中文**

# The other day

微信公众号「the other day」的官方网站。

用来存放我和朋友们的练习作品，顺便锻炼一下 HTML 相关的技能。
欢迎对编程提出任何建议——这是我的第一个仓库，经验很少，对网站的规范也完全没头绪。

## 目录结构

```
index.html          首页
basic_info.html     基础信息
members.html        现有人员
people/             成员个人页
category/           文章分类（年份 / 作者）
style.css           全站样式
header_bg.jpg       页头背景图
```

## 本地预览

指在**自己电脑上**打开页面查看效果，不经过 GitHub，也不经过线上部署。
改完立刻能看到，不用等 Pages 重建，也不会把半成品暴露到线上。

两种方式：

**1. 直接双击 `index.html`**

地址栏会显示 `file:///...`。纯静态页面用这个就够了，效果和线上基本一致。

**2. 起一个本地服务器**

```bash
python3 -m http.server 8000
```

然后访问 <http://localhost:8000/>。效果更接近线上（走的是 `http://` 而不是 `file://`），
以后如果加了需要读取文件的功能，`file://` 会被浏览器安全策略拦截，就必须用这种方式。

三种地址的区别：

| 地址 | 是什么 |
|---|---|
| `file:///.../html/index.html` | 硬盘上的文件，不走网络 |
| `http://localhost:8000/` | 本机临时服务器，只有自己能看到 |
| `https://chenyue321.github.io/The-other-day-website/` | 线上，所有人都能访问 |

修改流程：本地预览确认效果 → 提交 → 推送到 `main` → 等 Pages 重建（约一分钟）→ 线上更新。

## 许可

- **文字内容**：CC BY-NC-SA 4.0，全文见 [LICENSE](LICENSE)。
  可以转载和改编，但必须署名、不得用于商业目的、改编作品须使用相同协议。
- **代码**（HTML / CSS）：MIT，全文见 [LICENSE-CODE](LICENSE-CODE)。
  随便拿去用，出事别找我。

页头背景图 `header_bg.jpg` 如来自第三方，其版权归原作者所有，不在上述授权范围内。
