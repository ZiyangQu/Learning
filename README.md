# 线性代数学习笔记

这是一个使用 Jupyter Book 2 / MyST 构建的线性代数学习笔记项目，内容由 [`linear.txt`](./linear.txt) 整理而成。

## 本地预览

首次克隆后，在 PowerShell 中创建独立环境并安装依赖：

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

然后启动本地预览：

```powershell
.\.venv\Scripts\Activate.ps1
jupyter book start
```

## 构建网站

```powershell
jupyter book build --html --strict
```

构建结果位于 `_build/html`。推送到 `main` 分支后，GitHub Actions 会自动构建并发布 GitHub Pages。
