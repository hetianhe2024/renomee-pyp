# renomee-pyp

`renomee-pyp` 是一个 Python 包项目骨架（包名：`renomee_pyp`），并已配置 GitHub Actions + PyPI Trusted Publisher 的发布流程。

## 安装

```bash
python -m pip install renomee-pyp
```

## 使用

```python
import renomee_pyp

print(renomee_pyp.__version__)
```

## 发布到 PyPI（Trusted Publishing）

本仓库提供工作流：`.github/workflows/publish.yml`。

- 在 PyPI 的 “Trusted Publisher” 表单中：
  - **Owner**：`hetianhe2024`
  - **Repository name**：`renomee-pyp`
  - **Workflow name**：`publish.yml`
  - **Environment name**：留空（本工作流未使用 GitHub Environments）

触发方式：
- 发布一个 GitHub Release（`release: published` 会触发发布）
- 或者在 Actions 页面手动运行（`workflow_dispatch`）
