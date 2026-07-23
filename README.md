# 王悠然 · 个人网站

北京交通大学软件工程在读学生的个人主页，纯原生 HTML + CSS + Vanilla JS，零框架、零依赖。

线上地址：[https://youranwang-hub.github.io/personal-website](https://youranwang-hub.github.io/personal-website)

---

## 技术栈

| 类别 | 选型 |
|------|------|
| 标记 | HTML5 |
| 样式 | CSS3（自定义属性 + Flexbox） |
| 脚本 | Vanilla JavaScript（无第三方库） |
| 字体 | Georgia 衬线 + 系统无衬线混排 |
| 部署 | GitHub Pages |

## 页面结构

| 页面 | 说明 |
|------|------|
| `index.html` | 首页，聚合展示项目 / 论文 / 科研 / 爱好四大板块 |
| `projects.html` | 项目独立页，5 个项目卡片（可展开详情） |
| `papers.html` | 论文独立页，含竞赛论文展开详情 + 课程论文 |
| `research.html` | 科研独立页，2 个大创项目 |
| `hobbies.html` | 爱好页，摄影画廊（横向展开 + Lightbox 全屏）+ 吉他 |
| `project-new-meal.html` | 「上新了！我的饭」项目详情页 |
| `project-smart-logi.html` | 「智能物流配送终端」项目详情页 |
| `project-memolog.html` | 「Memolog」项目详情页 |

## 目录结构

```
personal-website/
├── index.html              # 首页
├── projects.html           # 项目页
├── papers.html             # 论文页
├── research.html           # 科研页
├── hobbies.html            # 爱好页
├── project-new-meal.html   # 项目详情：上新了！我的饭
├── project-smart-logi.html # 项目详情：智能物流配送终端
├── project-memolog.html    # 项目详情：Memolog
├── style.css               # 共享样式（约 900 行）
└── photos/                 # 摄影作品（6 张 JPG）
```

## 设计系统

**纸质感美学**，核心理念是"克制"。

### 配色

| 变量 | 色值 | 用途 |
|------|------|------|
| `--paper` | `#FAF8F5` | 米白底色 |
| `--ink` | `#2C2C2A` | 墨黑正文 |
| `--accent` | `#185FA5` | 蓝色强调（链接、标签） |
| `--accent-warm` | `#BA7517` | 暖色徽章（奖项） |

### 交互

- **翻页过渡**：点击导航链接时，overlay 从右滑入覆盖当前页，再跳转目标页
- **卡片展开**：点击项目/论文卡片展开详情，同时只展开一条，右侧三角图标旋转
- **hover 下划线**：标题下划线从左到右展开
- **摄影画廊**：横向 hover 展开 + Lightbox 全屏（支持键盘左右导航）
- **响应式**：`@media (max-width: 640px)` 适配移动端

### 布局

- 680px 居中窄栏
- 极细分隔线（0.5px）
- 留白克制，信息密度适中

## 本地运行

无需构建，直接用浏览器打开 `index.html` 即可。

或启动本地服务器：

```bash
# Python
python -m http.server 8080

# Node.js
npx serve
```

然后访问 `http://localhost:8080`。

## 站主

- **姓名**：王悠然
- **学校**：北京交通大学 · 软件工程 · 大二在读
- **GitHub**：[@youranwang-hub](https://github.com/youranwang-hub)
- **Email**：youranwang636@gmail.com

## License

&copy; 2026 王悠然. 保留所有权利。
