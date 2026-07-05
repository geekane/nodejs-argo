# AI 助手开发规范 (AI Coding Assistant Rules)

为了保证项目的正常运行和维护，所有 AI 编码助手在阅读和修改本项目代码时，必须严格遵守以下规则：

## 核心开发规则

1. **绝对禁止直接修改、覆盖或删除 `index.js`**
   - `index.js` 是部署时运行的最终混淆代码，由开发者手动或通过特定混淆工具基于源码生成。
   - AI 助手在任何情况下**都不要管、不要触碰、不要修改** `index.js`。

2. **所有源码逻辑修改均在 `index-oringal.js` 中进行**
   - `index-oringal.js` 是本项目唯一的未混淆干净源码。
   - 所有的功能开发、配置调整、错误修复等，**仅能且必须**在 [index-oringal.js](file:///d:/nodejs-argo/index-oringal.js) 中完成。

3. **依赖安装与包管理**
   - 本项目依赖已全面优化为轻量化的原生 `http` 模块，不再需要 `express` 依赖，请勿随意引入多余的 npm 第三方库。
