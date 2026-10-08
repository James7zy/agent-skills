# pstack 收录说明

本目录收录 `cursor/plugins` 中 `pstack/` 的完整快照，保留上游目录结构和文件内容，仅新增本说明，方便追踪来源和后续更新。

## 来源

- 上游项目：[cursor/plugins/pstack](https://github.com/cursor/plugins/tree/main/pstack)
- 插件版本：`0.15.15`
- 固定提交：[`ccb5507cec1546dc88135c1139c811e6c59115ba`](https://github.com/cursor/plugins/tree/ccb5507cec1546dc88135c1139c811e6c59115ba/pstack)
- 作者：Lauren Tan（poteto）
- 许可证：[MIT](LICENSE)

## 内容与入口

- `skills/`：51 个主 Skills（含工程原则），入口为 [poteto-mode](skills/poteto-mode/SKILL.md)。
- `agents/`：配套子代理定义。
- `docs/guide/`：[上手指南](docs/guide/README.md)。
- `automations/benny/`：可选自动化包，包含另外 3 个 Skills，默认不注册为斜杠命令。
- `.cursor-plugin/`、`assets/` 及各 Skill 的参考资料、工作流和脚本均按上游保留。

不确定从哪里开始时，阅读 [poteto-help](skills/poteto-help/SKILL.md) 或[上游 README](README.md)。按本工程的工作流使用时，将所选 `SKILL.md` 提供给 AI，并确保它能读取相邻的依赖文件。

## 环境依赖

本工程仅收录文件，不会自动安装 Cursor 插件、注册命令、修改用户配置或启用自动化。Cursor 的安装和使用步骤见[上游 README](README.md#install)。

完整工作流主要面向 Cursor：模型配置、子代理及部分工具依赖对应的运行环境。`deslop`、`control-cli` 和 `control-ui` 来自另一个 `cursor-team-kit` 插件，`create-skill` 是 Cursor 内置能力；本目录不包含这些依赖。在其他 AI 工具中使用时，需要适配相关调用，不能假定斜杠命令或子代理已可用。

## 更新

从选定的上游提交同步整个 `pstack/` 目录，保留本说明，并同步更新这里的版本、提交和内容统计。保持上游文件原样，避免移动单个 Skill 导致相对引用失效。
