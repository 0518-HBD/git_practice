# 客服机器人配置协作

本目录用于练习团队配置变更、Pull Request、代码审查、冲突解决、版本发布与回退。

## 初始配置

- app_name：应用名称，初始值为 SupportBot。
- welcome_message：欢迎语，初始值为 Hello。
- history_enabled：是否启用聊天历史，初始值为 false。
- history_limit：历史记录数量上限，初始值为 10。

这是配置协作项目，尚未实现机器人业务功能。

## 验证

在仓库根目录使用 Python 3 执行：

    python -m json.tool team_lab/config.json

该命令检查 JSON 语法。每次变更还需核对需求规定的配置值，并在 PR 中记录验证结果。

## 协作约定

- master 为本案例的主干；业务修改从最新主干创建任务分支，通过 PR 合并。
- 每次提交聚焦一个明确任务，合并前检查差异和验证结果。
- 本案例的 PR 统一使用 Create a merge commit，保留分支历史。
- .idea、虚拟环境、日志及本地密钥配置不纳入提交。
