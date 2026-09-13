# Markdown 美化指南 · Awesome Markdown Tips

[![GitHub stars](https://img.shields.io/github/stars/22ABLE22/awesome-markdown-tips?style=social)](https://github.com/22ABLE22/awesome-markdown-tips/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/22ABLE22/awesome-markdown-tips?style=social)](https://github.com/22ABLE22/awesome-markdown-tips/network/members)
[![GitHub watchers](https://img.shields.io/github/watchers/22ABLE22/awesome-markdown-tips?style=social)](https://github.com/22ABLE22/awesome-markdown-tips/watchers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> 一份可直接复制粘贴的 GitHub Markdown 美化速查表：徽章、统计卡片、折线图、图标、折叠块、表格、高亮块……一网打尽。

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=4000&pause=1000&color=39C5BB&center=true&vCenter=true&multiline=true&repeat=true&width=600&height=80&lines=Hello%2C+GitHub!;Welcome+to+Markdown+Tips;Star+this+repo+if+helpful" alt="Typing SVG" />
</p>

---

## 目录

- [1. Shields.io 徽章](#1-shieldsio-徽章)
- [2. 动态统计卡片](#2-动态统计卡片)
- [3. Star 历史折线图](#3-star-历史折线图)
- [4. 访客计数器](#4-访客计数器)
- [5. 打字机 / 标题动效](#5-打字机--标题动效)
- [6. 技术栈图标](#6-技术栈图标)
- [7. Markdown 结构技巧](#7-markdown-结构技巧)
- [8. 高亮引用块](#8-高亮引用块)
- [9. 进度条与百分比](#9-进度条与百分比)
- [10. 代码高亮与折叠](#10-代码高亮与折叠)
- [11. 表格进阶](#11-表格进阶)
- [12. 目录锚点技巧](#12-目录锚点技巧)
- [13. 复制即用模板](#13-复制即用模板)
- [14. 参考资源](#14-参考资源)

---

## 1. Shields.io 徽章

最常用的徽章服务：[shields.io](https://shields.io)

### 1.1 静态徽章

```markdown
![Static Badge](https://img.shields.io/badge/Python-%3E%3D3.10-blue)
![Static Badge](https://img.shields.io/badge/Status-Stable-brightgreen)
![Static Badge](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey)
```

效果：

![Static Badge](https://img.shields.io/badge/Python-%3E%3D3.10-blue)
![Static Badge](https://img.shields.io/badge/Status-Stable-brightgreen)
![Static Badge](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey)

### 1.2 点击跳转徽章

```markdown
[![Python](https://img.shields.io/badge/Python-%3E%3D3.10-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
```

效果：

[![Python](https://img.shields.io/badge/Python-%3E%3D3.10-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

### 1.3 常用颜色

| 颜色名 | 示例 | 十六进制 |
|--------|------|----------|
| `blue` | ![](https://img.shields.io/badge/blue-blue) | `#007ec6` |
| `brightgreen` | ![](https://img.shields.io/badge/brightgreen-brightgreen) | `#4c1` |
| `green` | ![](https://img.shields.io/badge/green-green) | `#97ca00` |
| `yellow` | ![](https://img.shields.io/badge/yellow-yellow) | `#dfb317` |
| `orange` | ![](https://img.shields.io/badge/orange-orange) | `#fe7d37` |
| `red` | ![](https://img.shields.io/badge/red-red) | `#e05d44` |
| `lightgrey` | ![](https://img.shields.io/badge/lightgrey-lightgrey) | `#9f9f9f` |
| `success` | ![](https://img.shields.io/badge/success-success) | `#4c1` |
| `important` | ![](https://img.shields.io/badge/important-important) | `#fe7d37` |
| `critical` | ![](https://img.shields.io/badge/critical-critical) | `#e05d44` |
| `informational` | ![](https://img.shields.io/badge/informational-informational) | `#007ec6` |
| `inactive` | ![](https://img.shields.io/badge/inactive-inactive) | `#9f9f9f` |

也支持自定义颜色：`https://img.shields.io/badge/label-message-39C5BB`

### 1.4 常用风格 Style

```
?style=flat          # 默认
?style=flat-square   # 直角
?style=plastic       # 塑料立体感
?style=for-the-badge # 大写大徽章
?style=social        # 社交风格（适合 stars/followers）
```

```markdown
![flat](https://img.shields.io/badge/style-flat-39C5BB?style=flat)
![flat-square](https://img.shields.io/badge/style-flat--square-39C5BB?style=flat-square)
![plastic](https://img.shields.io/badge/style-plastic-39C5BB?style=plastic)
![for-the-badge](https://img.shields.io/badge/STYLE-FOR--THE--BADGE-39C5BB?style=for-the-badge)
![social](https://img.shields.io/badge/style-social-39C5BB?style=social)
```

效果：

![flat](https://img.shields.io/badge/style-flat-39C5BB?style=flat)
![flat-square](https://img.shields.io/badge/style-flat--square-39C5BB?style=flat-square)
![plastic](https://img.shields.io/badge/style-plastic-39C5BB?style=plastic)
![for-the-badge](https://img.shields.io/badge/STYLE-FOR--THE--BADGE-39C5BB?style=for-the-badge)
![social](https://img.shields.io/badge/style-social-39C5BB?style=social)

### 1.5 动态徽章（自动读取仓库信息）

```markdown
![GitHub release](https://img.shields.io/github/v/release/OWNER/REPO)
![GitHub license](https://img.shields.io/github/license/OWNER/REPO)
![GitHub last commit](https://img.shields.io/github/last-commit/OWNER/REPO)
![GitHub issues](https://img.shields.io/github/issues/OWNER/REPO)
![GitHub pull requests](https://img.shields.io/github/issues-pr/OWNER/REPO)
![GitHub repo size](https://img.shields.io/github/repo-size/OWNER/REPO)
![GitHub code size](https://img.shields.io/github/languages/code-size/OWNER/REPO)
![GitHub stars](https://img.shields.io/github/stars/OWNER/REPO?style=social)
![GitHub forks](https://img.shields.io/github/forks/OWNER/REPO?style=social)
![GitHub language count](https://img.shields.io/github/languages/count/OWNER/REPO)
![Top language](https://img.shields.io/github/languages/top/OWNER/REPO)
```

### 1.6 平台 / 工具徽章

```markdown
![npm](https://img.shields.io/npm/v/react)
![npm downloads](https://img.shields.io/npm/dm/react)
![PyPI](https://img.shields.io/pypi/v/requests)
![Python versions](https://img.shields.io/pypi/pyversions/requests)
![Docker pulls](https://img.shields.io/docker/pulls/library/python)
![Discord](https://img.shields.io/discord/XXXXXXX)
![Twitter Follow](https://img.shields.io/twitter/follow/username)
```

### 1.7 自定义 Logo 徽章

在 URL 后加 `&logo=名称`：

```markdown
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
```

效果：

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

完整 logo 列表见：[simpleicons.org](https://simpleicons.org/)

### 1.8 第三方徽章服务

shields.io 不原生支持渐变，可用：

- [badgen.net](https://badgen.net)
- [flat-badges](https://github.com/bokub/flat-badges)

```markdown
![badgen](https://badgen.net/badge/Hello/World/blue)
```

---

## 2. 动态统计卡片

### 2.1 GitHub Stats（最流行）

来自 [github-readme-stats](https://github.com/anuraghazra/github-readme-stats)

```markdown
![GitHub stats](https://github-readme-stats.vercel.app/api?username=22ABLE22&show_icons=true&theme=radical)
```

效果（把 `22ABLE22` 换成你的）：

![GitHub stats](https://github-readme-stats.vercel.app/api?username=github&show_icons=true&theme=radical)

#### 主题列表

| 主题名 | 主题名 | 主题名 |
|--------|--------|--------|
| `dark` | `radical` | `merko` |
| `gruvbox` | `tokyonight` | `onedark` |
| `cobalt` | `synthwave` | `highcontrast` |
| `dracula` | `prussian` | `monokai` |
| `vue` | `vue-dark` | `shades-of-purple` |
| `nightowl` | `buefy` | `blue-green` |
| `algolia` | `great-gatsby` | `darcula` |
| `bear` | `solarized-dark` | `solarized-light` |
| `gotham` | `material-palenight` | `graywhite` |
| `ayu-mirage` | `midnight-purple` | `calm` |
| `omni` | `react` | `jolly` |
| `github_dark` | `github_dark_dimmed` | `transparent` |

#### 常用参数

```
&show_icons=true          # 显示图标
&hide_border=true         # 隐藏边框
&hide_title=true          # 隐藏标题
&hide_rank=true           # 隐藏排名
&include_all_commits=true # 统计全部提交
&count_private=true       # 统计私有仓库（需 PAT）
&bg_color=0D1117          # 自定义背景
&title_color=39C5BB       # 标题色
&icon_color=39C5BB        # 图标色
&text_color=C9D1D9        # 文字色
&border_color=30363D      # 边框色
&ring_color=39C5BB        # 排名环颜色
&layout=compact           # 紧凑布局
&custom_title=My Stats    # 自定义标题
```

### 2.2 Top Languages 语言占比

```markdown
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=22ABLE22&layout=compact&theme=radical)
```

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=github&layout=compact&theme=radical)

参数：

```
&layout=compact           # 紧凑（默认 card）
&langs_count=8            # 显示语言数量（默认 5）
&hide=html,css            # 隐藏某些语言
&exclude_repo=repo1,repo2 # 排除仓库
&size_weight=0.5          # 按代码量加权
&count_weight=0.5         # 按提交数加权
```

### 2.3 Wakatime 编程时长

需要绑定 [WakaTime](https://wakatime.com)：

```markdown
[![WakaTime](https://github-readme-stats.vercel.app/api/wakatime?username=22ABLE22&theme=radical)](https://wakatime.com/@22ABLE22)
```

### 2.4 Profile Summary Card

```markdown
[![Profile Summary Card](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=22ABLE22&theme=radical)](https://github.com/vn7n24fzkq/github-profile-summary-cards)
[![Profile Summary Card](https://github-profile-summary-cards.vercel.app/api/cards/stats?username=22ABLE22&theme=radical)](https://github.com/vn7n24fzkq/github-profile-summary-cards)
```

### 2.5 GitHub Activity Graph 活跃图

```markdown
[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=22ABLE22&theme=react-dark)](https://github.com/ashutosh00710/github-readme-activity-graph)
```

主题：`react` / `react-dark` / `github` / `github-compact` / `xcode` / `rogue` / `toastedmarshmallow` 等

### 2.6 Streak Stats 连续提交

```markdown
[![GitHub Streak](https://streak-stats.demolab.com?user=22ABLE22&theme=radical)](https://git.io/streak-stats)
```

![GitHub Streak](https://streak-stats.demolab.com?user=github&theme=radical)

---

## 3. Star 历史折线图

### 3.1 Star History（推荐）

```markdown
[![Star History Chart](https://api.star-history.com/svg?repos=22ABLE22/awesome-markdown-tips&type=Date)](https://star-history.com/#22ABLE22/awesome-markdown-tips&Date)
```

### 3.2 对比多个仓库

```markdown
[![Star History Chart](https://api.star-history.com/svg?repos=facebook/react,vuejs/core&type=Date)](https://star-history.com/#facebook/react&vuejs/core&Date)
```

### 3.3 其他图表服务

```markdown
<!-- RepoBeats -->
[![RepoBeats](https://repobeats.axiom.co/api/embed/22ABLE22/awesome-markdown-tips.svg)](https://repobeats.axiom.co)
```

### 3.4 贡献者图片墙

```markdown
[![Contributors](https://contrib.rocks/image?repo=22ABLE22/awesome-markdown-tips)](https://github.com/22ABLE22/awesome-markdown-tips/graphs/contributors)
```

参数：

```
?max=21          # 最多显示人数
&anon=true       # 显示匿名贡献者
```

---

## 4. 访客计数器

### 4.1 Profile Views（社区版）

```markdown
![Profile views](https://komarev.com/ghpvc/?username=22ABLE22&color=brightgreen)
```

![Profile views](https://komarev.com/ghpvc/?username=github&color=brightgreen)

参数：

```
&color=blue|green|red|...  # 颜色
&style=flat|plastic        # 风格
&label=Profile views       # 自定义标签
```

### 4.2 Hit Counter（另一方案）

```markdown
![Visitor Count](https://hits.sh/github.com/22ABLE22/awesome-markdown-tips.svg?color=39C5BB&label=Visitors)
```

### 4.3 在线人数（Discord 风格）

```markdown
![Discord](https://img.shields.io/discord/SERVER_ID?label=Discord&logo=discord)
```

---

## 5. 打字机 / 标题动效

### 5.1 Readme Typing SVG

```markdown
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=4000&pause=1000&color=39C5BB&center=true&vCenter=true&multiline=true&repeat=true&width=600&height=80&lines=Hello%2C+I+am+Alice;Full-stack+Developer;Open+Source+Lover" alt="Typing SVG" />
</p>
```

参数说明：

| 参数 | 说明 |
|------|------|
| `font` | 字体（Fira Code, JetBrains Mono, Pacifico 等） |
| `weight` | 字重 |
| `size` | 字号 |
| `duration` | 每行打字时长 ms |
| `pause` | 行间停顿 ms |
| `color` | 颜色 hex 或名称 |
| `center` | 水平居中 |
| `vCenter` | 垂直居中 |
| `multiline` | 支持多行 |
| `repeat` | 循环播放 |
| `width` / `height` | 画布尺寸 |
| `lines` | 句子，用 `;` 分隔（需 URL 编码） |

### 5.2 Header SVG

```markdown
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:39C5BB,100:1a7f8f&height=200&section=header&text=My%20Profile&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Full-stack%20Developer&descSize=20&descAlignY=60" />
</p>
```

### 5.3 Capsule Render 底部

```markdown
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:39C5BB,100:1a7f8f&height=180&section=footer" />
</p>
```

### 5.4 常用 capsule type

```
type=wave      # 波浪
type=waving    # 动态波浪
type=rounded   # 圆角矩形
type=slice     # 切片
type=rect      # 矩形
type=soft      # 柔和
type=stripe    # 条纹
type=venom     # 毒液风格
type=transparent
type=auto      # 自动
type=cylinder
type=egg
type=shark
type=amoled
```

---

## 6. 技术栈图标

### 6.1 Skill Icons（推荐）

[skillicons.dev](https://skillicons.dev)

```markdown
![My Skills](https://skillicons.dev/icons?i=js,ts,html,css,react,vue,nodejs,express,python,django,java,spring,cpp,go,postgres,mysql,redis,graphql,docker,aws,gcp,azure,linux,git,github,vercel,netlify,idea,vscode,figma&perline=8)
```

![My Skills](https://skillicons.dev/icons?i=js,ts,html,css,react,vue,nodejs,python,django,docker,git,github,vscode,linux,postgres,redis&perline=8)

可用图标名称示例：

```
js ts html css sass react vue nodejs nextjs express
python django flask java spring cpp c go rust
docker kubernetes aws gcp azure linux ubuntu
git github gitlab vscode idea vim
mysql postgres mongodb redis graphql
figma blender photoshop electron
tensorflow pytorch pandas numpy
nginx redis firebase vercel netlify
```

### 6.2 Shields.io + Simple Icons（for-the-badge 一排）

```markdown
<p align="center">
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  </a>
  <a href="https://react.dev/">
    <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  </a>
</p>
```

### 6.3 Devicons

```markdown
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="48" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" width="48" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="48" />
```

---

## 7. Markdown 结构技巧

### 7.1 折叠详情（`<details>`）

```markdown
<details>
  <summary>点击展开更多细节</summary>

  这里是隐藏的内容。

  - 支持 Markdown
  - 支持代码块
  - 支持图片

</details>
```

效果：

<details>
  <summary>点击展开更多细节</summary>

  这里是隐藏的内容。

  - 支持 Markdown
  - 支持代码块
  - 支持图片

</details>

**注意：** `<summary>` 后必须空一行再写正文，否则内容不会正确渲染。

### 7.2 默认展开

```markdown
<details open>
  <summary>默认展开</summary>

  内容…

</details>
```

### 7.3 HTML 对齐

```markdown
<p align="center">居中文本</p>
<p align="right">右对齐文本</p>
<div align="center">
  <img src="..." width="400" />
</div>
```

### 7.4 分割线

```markdown
---
***
___
```

### 7.5 换行

```markdown
第一行末尾加两个空格  
然后换行

或者直接空一行分段
```

---

## 8. 高亮引用块

### 8.1 基础引用

```markdown
> 这是一段引用文字
```

### 8.2 GitHub 原生提示块

```markdown
> [!NOTE]
> 有用的信息，用户应当知道。

> [!TIP]
> 更好的做法或有用技巧。

> [!IMPORTANT]
> 用户成功使用本产品必须知道的关键信息。

> [!WARNING]
> 可能出现问题，需要立即关注。

> [!CAUTION]
> 某些行为可能造成负面后果。
```

效果：

> [!NOTE]
> 有用的信息，用户应当知道。

> [!TIP]
> 更好的做法或有用技巧。

> [!IMPORTANT]
> 用户成功使用本产品必须知道的关键信息。

> [!WARNING]
> 可能出现问题，需要立即关注。

> [!CAUTION]
> 某些行为可能造成负面后果。

### 8.3 自定义彩色框（HTML）

```markdown
<table>
  <tr>
    <td>⚠️</td>
    <td><b>警告：</b>此操作不可逆！</td>
  </tr>
</table>
```

---

## 9. 进度条与百分比

### 9.1 文字进度条

```
![img](https://progress-bar.xyz/75/?title=进度&width=200&color=39C5BB)
```

效果：

![img](https://progress-bar.xyz/75/?title=进度&width=200&color=39C5BB)

### 9.2 多技能条（用徽章模拟）

```markdown
<img src="https://img.shields.io/badge/JavaScript-90%25-yellow?style=flat-square" />
<img src="https://img.shields.io/badge/Python-85%25-blue?style=flat-square" />
<img src="https://img.shields.io/badge/Docker-70%25-blue?style=flat-square" />
```

效果：

![JavaScript](https://img.shields.io/badge/JavaScript-90%25-yellow?style=flat-square)
![Python](https://img.shields.io/badge/Python-85%25-blue?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-70%25-blue?style=flat-square)

### 9.3 纯文本进度条

```
Python    ████████████████████░░░░░  80%
JS        ██████████████████████░░░  90%
Docker    ██████████████░░░░░░░░░░░  60%
```

---

## 10. 代码高亮与折叠

### 10.1 语法高亮

````markdown
```python
def hello(name: str) -> str:
    return f"Hello, {name}!"
```

```javascript
const greet = (name) => `Hello, ${name}!`;
```

```bash
git clone https://github.com/owner/repo.git
```

```diff
- 删除的行
+ 新增的行
```
````

### 10.2 命令行高亮

````markdown
```console
$ pip install awesome-package
Successfully installed awesome-package-1.0.0
```
````

---

## 11. 表格进阶

### 11.1 对齐

```markdown
| 左对齐 | 居中 | 右对齐 |
|:-------|:----:|-------:|
| a      |  b   |      c |
| ddddd  | eeee |   ffff |
```

| 左对齐 | 居中 | 右对齐 |
|:-------|:----:|-------:|
| a      |  b   |      c |
| ddddd  | eeee |   ffff |

### 11.2 表格内换行

```markdown
| 列 A | 列 B |
|------|------|
| 第一行<br>第二行 | 多行文本<br>用 `<br>` |
```

| 列 A | 列 B |
|------|------|
| 第一行<br>第二行 | 多行文本<br>用 `<br>` |

### 11.3 表格内嵌徽章 / 图片

```markdown
| 徽章 | 说明 |
|------|------|
| ![Python](https://img.shields.io/badge/Python-3.10+-blue) | Python 版本要求 |
```

---

## 12. 目录锚点技巧

### 12.1 自动目录（靠标题生成）

GitHub 会根据标题自动生成锚点：

- 中文标题：`#1-shieldsio-徽章`
- 英文标题：小写、空格变 `-`、去掉标点
- 重复标题：自动加 `-1` `-2`

### 12.2 手动锚点

```markdown
<a name="my-anchor"></a>
### 任意标题

[跳转到锚点](#my-anchor)
```

### 12.3 回到顶部

```markdown
<div align="right">

[![Back to top](https://img.shields.io/badge/%E2%AC%86%EF%B8%8F_Back_to_top-39C5BB?style=for-the-badge)](#)

</div>
```

---

## 13. 复制即用模板

### 13.1 个人 Profile README 片段

```markdown
# Hi there, I'm Alice 👋

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=800&color=39C5BB&center=true&vCenter=true&lines=Full-stack+Developer;Open+Source+Enthusiast)](https://git.io/typing-svg)

### 🔭 I'm currently working on
- Something amazing with React & Python

### 🌱 I'm currently learning
- Rust · WebAssembly · LLM Ops

### 🤝 I'm looking for
- Open source collaboration

### 📫 How to reach me
[![Email](https://img.shields.io/badge/Email-alice%40example.com-blue?style=flat-square&logo=gmail)](mailto:alice@example.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/alice)

---

### 📊 GitHub Stats

![Alice's GitHub stats](https://github-readme-stats.vercel.app/api?username=alice&show_icons=true&theme=radical)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=alice&layout=compact&theme=radical)

[![GitHub Streak](https://streak-stats.demolab.com?user=alice&theme=radical)](https://git.io/streak-stats)

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=alice&theme=react-dark)](https://github.com/ashutosh00710/github-readme-activity-graph)

---

### 🛠️ Tech Stack

![My Skills](https://skillicons.dev/icons?i=js,ts,react,python,django,docker,git,github,vscode,linux,postgres,redis&perline=6)
```

### 13.2 项目 README 片段

```markdown
<div align="center">

# 🚀 My Awesome Project

[![Release](https://img.shields.io/github/v/release/OWNER/REPO?include_prereleases&sort=semver)](https://github.com/OWNER/REPO/releases)
[![License](https://img.shields.io/github/license/OWNER/REPO)](https://github.com/OWNER/REPO/blob/main/LICENSE)
[![Build](https://img.shields.io/github/actions/workflow/status/OWNER/REPO/ci.yml)](https://github.com/OWNER/REPO/actions)
[![Stars](https://img.shields.io/github/stars/OWNER/REPO?style=social)](https://github.com/OWNER/REPO/stargazers)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3500&pause=1000&color=39C5BB&center=true&vCenter=true&multiline=true&lines=One+liner+description;Install+in+30+seconds)](https://git.io/typing-svg)

[English](./README.md) | [简体中文](./README.zh-CN.md)

</div>

## ✨ Features

- Feature 1
- Feature 2

## 📦 Installation

```bash
pip install my-awesome-project
```

## 🚀 Quick Start

```python
from my_awesome_project import hello

print(hello("world"))
```

## 📊 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=OWNER/REPO&type=Date)](https://star-history.com/#OWNER/REPO&Date)

## 🤝 Contributors

[![Contributors](https://contrib.rocks/image?repo=OWNER/REPO)](https://github.com/OWNER/REPO/graphs/contributors)

## 📄 License

[MIT](./LICENSE)
```

---

## 14. 参考资源

### 服务 / 生成器

| 名称 | 用途 | 链接 |
|------|------|------|
| Shields.io | 徽章 | https://shields.io |
| Simple Icons | 品牌 logo | https://simpleicons.org |
| github-readme-stats | 统计卡片 | https://github.com/anuraghazra/github-readme-stats |
| streak-stats | 连续提交 | https://github.com/DenverCoder1/github-readme-streak-stats |
| github-readme-activity-graph | 活跃图 | https://github.com/Ashutosh00710/github-readme-activity-graph |
| readme-typing-svg | 打字机 | https://github.com/DenverCoder1/readme-typing-svg |
| capsule-render | 波浪页眉页脚 | https://github.com/kyechan99/capsule-render |
| skillicons | 技术图标 | https://skillicons.dev |
| star-history | Star 折线图 | https://star-history.com |
| contrib.rocks | 贡献者墙 | https://contrib.rocks |
| profile-summary-cards | 概览卡片 | https://github.com/VN7N24FZKQ/github-profile-summary-cards |
| komarev | 访客计数 | https://komarev.com/ghpvc/ |
| all-contributors | 贡献者徽章 | https://allcontributors.org |
| awesome-badges | 徽章大全 | https://github.com/ileriayo/awesome-badges |

### Markdown 规范

- [GitHub Flavored Markdown](https://docs.github.com/en/get-started/writing-on-github)
- [CommonMark Spec](https://commonmark.org/)

---

<div align="center">

**如果这个仓库对你有帮助，请给一个 ⭐ Star！**

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:39C5BB,100:1a7f8f&height=120&section=footer)

</div>
