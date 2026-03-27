# deep_pytorch

## 推荐：Conda / Mamba 环境（可复现）

在项目根目录执行：

```bash
conda env create -f environment.yml
conda activate deep_pytorch
python -m ipykernel install --user --name deep_pytorch --display-name "deep_pytorch (Py3.12)"
```

然后在 Notebook 里把 kernel 切换到：`deep_pytorch (Py3.12)`。

更新环境（改了 `environment.yml` 之后）：

```bash
conda env update -f environment.yml --prune
```

## 备选：纯 pip + venv

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -U pip
python -m pip install -r requirements.txt
python -m ipykernel install --user --name deep_pytorch_venv --display-name "deep_pytorch (venv)"
```

## 快速自检

```bash
python -c "import torch; print(torch.__version__)"
```
