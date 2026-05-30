# TacView·AI — 智能战术场景编辑器

基于 RAG + DeepSeek + BGE-M3 的 AI 场景生成系统，个人独立全栈开发。

用自然语言描述作战意图，后端检索战术知识库并调用 DeepSeek 生成结构化场景数据，前端通过 postMessage 注入 iframe 内嵌地图编辑器实时渲染，最终可导出标准 ACMI 文件对接 TacView 仿真软件。

知识库由 4 个 Markdown 文档构成，覆盖实体类型规范、战术场景模板、数据链与雷达配置、JSON 输出格式约束，支持新增文档后重启自动加载。后端基于 Flask 提供场景生成、健康检查、知识库查看等接口，前端为原生 HTML + JS 实现的对话式界面。# tacview-
