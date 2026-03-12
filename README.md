# My Skills

这是我的自定义 Claude Code Skills 仓库。

## 包含的 Skills

### tech-blog-writer

生成结构化的技术博客文章，包含代码示例、最佳实践和清晰的解释。

**使用方法**：
```
/tech-blog-writer JavaScript 闭包详解
```

**特性**：
- 自动生成文章结构
- 包含代码示例和注释
- 遵循最佳写作实践
- 提供模板和示例参考

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

## 如何使用

1. 在 cc-switch 中添加此仓库
2. 启用需要的 skills
3. 使用 `/skill-name` 命令调用

## 目录结构

```
My-skills/
├── README.md
├── tech-blog-writer/
│   ├── SKILL.md
│   ├── templates/
│   │   └── blog-template.md
│   └── examples/
│       └── javascript-closure-example.md
└── learning-notes/
    ├── SKILL.md
    ├── templates/
    │   └── note-template.md
    └── examples/
        └── react-hooks-example.md
```
