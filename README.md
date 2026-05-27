# Manta-Learning-Journal

用静态 HTML 记录学习过程，并把值得反复查看的结论做成可直接访问的页面。

## 站点结构

```
.
├── index.html
├── notes/
│   ├── index.html
│   └── nvidia_deep_learning_tools/
│       └── index.html
└── README.md
```

- `index.html`：站点首页，负责导航和精选入口。
- `notes/index.html`：笔记归档页，集中展示全部内容。
- `notes/<slug>/index.html`：单篇笔记的规范路径。

## 在线访问

- 首页：<https://mantastack.github.io/Manta-Learning-Journal/>
- 笔记归档：<https://mantastack.github.io/Manta-Learning-Journal/notes/>
- NVIDIA 深度学习工具全景图：<https://mantastack.github.io/Manta-Learning-Journal/notes/nvidia_deep_learning_tools/>

## 发布

如果 GitHub Pages 已经配置为从 `main` 分支根目录发布，日常发布只需要：

```bash
git add .
git commit -m "Reorganize site structure"
git push origin main
```

后续新增内容建议直接放到 `notes/<slug>/index.html`，并在首页和归档页补导航入口。
