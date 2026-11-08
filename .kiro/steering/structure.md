# 小新AI资讯工具站 - 文件结构

## 当前项目结构

```
task/
├── index.html          # 单文件网站（HTML + CSS + JS）
└── .kiro/              # Kiro配置目录
    ├── steering/       # 项目规范文件
    │   ├── product.md  # 产品说明
    │   ├── tech.md     # 技术栈文档
    │   └── structure.md # 本文件
    └── specs/          # Kiro规格文档
        └── ai-news-tools-site/
            ├── requirements.md  # 需求文档
            ├── design.md        # 设计文档
            └── tasks.md         # 任务清单
```

## index.html结构说明

### CSS样式组织（按功能模块）

1. **CSS变量** - 主题色、响应式断点
2. **全局样式** - 重置、排版、颜色
3. **导航** - `.nav`、`.brand`、`.nav nav a`
4. **Hero区** - `.hero`、`.hero-grid`、`.hero-img`、`.stats`
5. **通用模块** - `.sec-head`、`.filters`、`.searchbox`
6. **资讯模块** - `.featured`、`.grid`、`.card`、`.tag`、`.meta`
7. **工具模块** - `.tool-ic`、`.free-note`
8. **羊毛模块** - `.deal`、`.amt`、`.us`
9. **提示词工坊** - `.panel`、`.form-grid`、`.inp`、`.hint`、`.titles`
10. **选题助手** - `.cmp`
11. **参赛提交包** - `.pack`、`.full`、`.steps`、`.step`
12. **页脚** - `footer`
13. **提示框** - `.toast`

### JavaScript功能

1. **主题切换** - 点击切换亮暗色
2. **搜索过滤** - 资讯关键词搜索与标签过滤
3. **提示词生成** - 在线生成提示词
4. **选题生成** - 生成短视频标题
5. **复制功能** - Devpost模板复制

## 响应式设计

- 桌面端（>860px）：多列布局
- 平板/移动端（≤860px）：单列布局
- 适配移动端视口（viewport-fit=cover）