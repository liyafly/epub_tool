# 下一步计划（new-tools）

1. 完成 `packages/core` 的 EPUB 解析/打包基础实现（jszip + fast-xml-parser，mimetype STORE 写入）。
2. 补上 `tool-checker.ts` 以检测 Node/Python/Rust/jpegoptim/oxipng 等依赖，并接入 CLI `doctor`。
3. 在 core 中落地 `epub/reformat.ts` 与 `image/webp-converter.ts` 的最小可运行版本，供 CLI 端到端验证。
4. 对 CLI 增补 `reformat`/`convert-webp`/`encrypt`/`decrypt` 子命令的参数校验和日志输出。
5. 为上述模块添加 smoke 测试/示例脚本（优先覆盖 EPUB 解包-重打包和路径映射正确性）。
