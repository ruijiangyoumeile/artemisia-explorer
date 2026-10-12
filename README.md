# 艾草 · 形与香

公开体验：https://ruijiangyoumeile.github.io/artemisia-explorer/

使用 Three.js 的三维科普页面，支持整体、叶片、叶背、茎和根的镜头聚焦，以及香气、文化资料。

## 发布与更新

GitHub Pages 从 main 分支根目录发布。后续版本直接更新本仓库，网站地址保持不变。发布新版时更新 index.html 中 app.js/style.css 的版本参数，以及 app.js 中模型 URL 的版本参数，避免浏览器沿用旧资源。等待 Pages 部署成功后再验收；CDN 缓存传播可能存在短暂延迟。

## 模型优化

采用 Draco 几何压缩与 WebP 纹理，模型资源从约 36.5 MB 降为 3.2 MB，减少约 91%；保留原有三角面。法线与材质图为 1024，颜色图为 2048。模型没有独立分件，当前版本采用镜头聚焦。

## 知识与许可

以 Artemisia argyi 为科普对象，但所给模型尚未经物种鉴定。形态、器官功能、叶精油和文化资料均在页面中列出来源。叶部研究不套用到茎或根，传统用途不等同于临床疗效。

模型由用户提供。Three.js 使用 MIT 许可，见 THREE-LICENSE.txt。交互思路参考 nytimes/three-story-controls 与 donmccurdy/three-gltf-viewer，未复制参考项目代码。
