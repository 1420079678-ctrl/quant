# quant

A 股数据与量化分析的 Python 项目，用 [uv](https://docs.astral.sh/uv/) 管理，要求 Python 3.12 或更新版本。

## 现状

骨架阶段。`src/quant/__init__.py` 目前只有一个 `hello()` 示例函数，行情数据接入、指标计算与策略回测都还没有开始写。

## 依赖

| 包 | 用途 |
| --- | --- |
| akshare | A 股行情与基本面数据接口 |
| pandas / numpy | 数据处理与数值计算 |
| pyarrow | Parquet 列式存储 |
| matplotlib | 绘图 |

## 开始

```powershell
uv sync                                                    # 创建环境并安装依赖
uv run python -c "import quant; print(quant.hello())"      # 确认包可导入
```

## 结构

```text
src/quant/          包源码（src 布局，py.typed 已声明类型标记）
pyproject.toml      项目元数据与依赖
.venv/              本地虚拟环境，不入库
```
