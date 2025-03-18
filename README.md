# Jupyterlab Template

Jupyterlabのテンプレートレポジトリ

## Install Library

```bash
# 仮想環境の構築
python3 -m venv.venv

# 仮想環境の起動
source ./.venv/bin/activate

# Install Library
python3 -m pip install Jupyterlab \
  jupyterlab-language-pack-ja-JP \ # 日本語化
  jupyterlab-git \ # Git
  lckr_jupyterlab_variableinspector \
  jupyterlab-code-formatter \
  # (black or yapf or autopep8) \ # コード自動整形
  matplotlib \
  pandas numpy \
  # jupyter-ai[all] \
  jupyter-ai langchain-openai
  # jupyter_contrib_nbextensions \
  'jupyterlab>=4.0.0,<5.0.0a0' jupyterlab-lsp \
  # jedi-language-server \
  'python-lsp-server[all]' \
  polars \
  vaex \
  plotly \
  altair vega_datasets \
  pycaret \
  shap \
  seaborn \
  tensorflow[and cuda] \
  scikit-learn

# ライブラリの書き出し
python3 -m pip freeze > requirements.txt

# Jupyterlabの起動(ローカルホスト以外にも見えるように)
Jupyter-lab --ip='0.0.0.0' --NotebookApp.token=''
```


## 参考サイト

- [2024年最新版：Pythonデータ解析ライブラリ総まとめ - 実践的ガイド #機械学習 - Qiita](https://qiita.com/Tadataka_Takahashi/items/3f48b48c95b63f6d6ab7)
- [Start Locally | PyTorch](https://pytorch.org/get-started/locally/)
- [pip を使用して TensorFlow をインストールする ](https://www.tensorflow.org/install/pip?hl=ja)
- [Getting started with Keras](https://keras.io/getting_started/)
