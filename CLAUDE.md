# AI学习课程 项目规范

## 目录命名规范

```
01. 第一章 章节标题/
02. 第二章 章节标题/
...
```

每章目录内结构：

```
00. 导言.md
01. 第一节 节名.md
02. 第二节 节名.md
...
image/
  cover.png       # 章节封面图
  其他配图.png
```

## 导言文件结构

```markdown
# 第X章：标题

![cover](image/cover.png)

150-200字的章节导言，语气诙谐，点明本章核心主题，
最后一句作为钩子引出后续内容。
```

## 小节文件结构

```markdown
# 第X节：节名 —— 副标题

## 1. 小标题

正文内容

---

## 2. 小标题

正文内容

---

> [!NOTE]
> 一句话概括本节核心，放在文章末尾。
```

## 配图生成规范

**工具：** image2

**格式：** 中文场景描述 + 英文风格模板，用逗号连接。

**固定英文风格模板（每张图直接复制）：**

```
editorial illustration style,
flat design with soft rounded shapes, warm color palette,
subtle shadows, hand-drawn texture on edges,
generous whitespace, layered composition,
magazine layout aesthetic, high information density but not cluttered,
NO text, NO words, NO labels, NO numbers, NO letters,
pure visual storytelling, symbols and imagery only
```

**使用方法：**

```
[中文场景描述]
,
editorial illustration style,
flat design with soft rounded shapes, warm color palette,
subtle shadows, hand-drawn texture on edges,
generous whitespace, layered composition,
magazine layout aesthetic, high information density but not cluttered,
NO text, NO words, NO labels, NO numbers, NO letters,
pure visual storytelling, symbols and imagery only
```
