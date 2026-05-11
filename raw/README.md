# raw

这里放已经完成分流的原始资料。

这里默认是只读层。资料一旦导入完成，就不要在这里补总结、打标签、重写内容。

现在的默认流程不是“先把东西直接扔进 `raw/`”，而是：

1. 先进入 [[Clippings/README|Clippings/README.md]]
2. 判断它属于哪类原始来源
3. 再迁成 `raw/` 下的标准来源包

也就是说，`raw/` 负责长期保存，`Clippings/` 负责先接住新东西。

建议分到这些目录：

- `web/`：网页文章、博客、新闻、访谈，优先按来源包存
- `chats/`：聊天记录、会议纪要、私聊摘录、语音转写，先保原文和语境
- `papers/`：论文、技术报告
- `books/`：图书、成套教材、上下册文档
- `repos/`：代码仓库说明、关键源码摘录
- `datasets/`：数据集文档、说明页
- `images/`：独立图片来源

推荐结构不是“散文件”，而是“来源包”：

```text
raw/
  web/
    2026-04-13-some-article/
      some-article.md
      images/
      files/
      metadata.json
```

```text
raw/
  chats/
    2026-04-24-some-conversation/
      transcript.md
      attachments/
      metadata.md
```

```text
raw/
  papers/
    2024-some-paper/
      paper.pdf
      figures/
      metadata.json
```

维护原则：

- 尽量保留原始内容
- 不把总结写在这里
- 正文、图片、附件尽量放在同一个来源包里
- 网页、聊天或其他文本类来源的正文主文件默认用简短、直观的语义名；只有在容易撞名时才补最少的消歧尾巴
- 页面里带的图片不要单独拆到通用目录
- 对话型材料先保参与人、时间范围和引用边界，再考虑后续提炼
- 老目录结构先兼容，不强制改
- 如果某份材料最后发现并不适合做正式来源，不要硬塞进 `raw/`，而应改分流到 `seeds/` 或 `todo/`
