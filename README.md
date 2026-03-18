# My Skills

这是我的通用 Skills 仓库，可用于 Claude Code、Codex、Gemini 等支持 Skills 的工具。

## 包含的 Skills

### tech-blog-writer

生成结构化的技术博客、教程和开发者文章，包含代码示例、最佳实践和清晰解释。

**使用方法**：
```
/tech-blog-writer JavaScript 闭包详解
```

**特性**：
- 自动生成文章结构
- 包含代码示例和注释
- 遵循最佳写作实践
- 提供模板和示例参考
- 支持改写与润色现有草稿

---

### learning-notes

创建结构化的学习笔记，自动解释概念定义并建立知识点之间的联系。

**使用方法**：
```
/learning-notes JavaScript 闭包
/learning-notes 分析文件 ~/notes/react-hooks.md
```

**特性**：
- 自动识别和解释关键概念
- 建立概念之间的关联关系
- 生成概念关系图
- 提供实践练习和复习要点
- 支持从现有文件生成笔记

---

### analyze-article-sources

分析博客文章、报告或论文，输出摘要、文章结构，并为关键数据、事件和事实性主张补充来源链接。

**使用方法**：
```text
/analyze-article-sources 总结这篇文章并给出关键数据的来源链接
```

**特性**：
- 提取文章主旨和结构
- 识别需要核验的数据、事件和论文引用
- 优先查找一手或接近一手来源
- 输出 claim 到 source 的映射关系

## 如何使用

1. 在支持 Skills 的工具或管理器中添加此仓库
2. 启用需要的 skills
3. 使用 `/skill-name` 或显式 skill 调用方式触发

## 目录结构

```
My-skills/
├── README.md
├── analyze-article-sources/
│   ├── SKILL.md
│   ├── agents/
│   │   └── openai.yaml
│   └── references/
│       └── source-priority.md
├── tech-blog-writer/
│   ├── SKILL.md
│   ├── agents/
│   │   └── openai.yaml
│   ├── templates/
│   │   └── blog-template.md
│   └── examples/
│       └── javascript-closure-example.md
└── learning-notes/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    ├── templates/
    │   └── note-template.md
    └── examples/
        └── react-hooks-example.md
```
