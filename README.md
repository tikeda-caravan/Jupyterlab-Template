# Jupyterlab Template

Jupyterlabのテンプレートレポジトリ

## Install Library

### Windows

```powershell
# 仮想環境の構築
python -m venv .venv

# PowerShell の実行ポリシーの確認と設定
# 実行ポリシーの確認
# Undefinedの出力の場合変更が必要になる
Get-ExecutionPolicy -Scope CurrentUser

# 実行ポリシーを RemoteSigned に変更する
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser RemoteSigned

# 仮想環境の起動
.\.venv\Scripts\activate

# Install Library
python -m pip \
  
  # Jupyterlab
  install Jupyterlab \
  
  # Jupyterlabの日本語化
  jupyterlab-language-pack-ja-JP \
  
  # 拡張機能を追加する拡張機能
  # jupyter_contrib_nbextensions \
  
  # JupyterlabのGit拡張機能
  jupyterlab-git \
  
  # 変数の確認するための拡張機能
  lckr_jupyterlab_variableinspector \
  
  # Pythonコードのフォーマッター
  jupyterlab-code-formatter \
  
  # コード補完機能
  'jupyterlab>=4.0.0,<5.0.0a0' jupyterlab-lsp \

  # コード自動整形
  # jedi-language-server \
  # 'python-lsp-server[all]' \
  'python-lsp-server[autopep8]' \
  # autopep8 \
  
  # ChatGPTの拡張機能
  # jupyter-ai[all] \
  jupyter-ai langchain-openai
  
  # Data Science
  matplotlib \
  pandas \
  numpy \
  polars \
  plotly \
  seaborn \
  scikit-learn \
  tensorflow[and cuda] \
  pycaret \
  shap \
  
  # vaex: BigData向けのpandasの似たライブラリ
  vaex \
  # altair: データ可視化ライブラリ
  altair \
  # vega_dataset: altairとセットで使われるデータセットがあるライブラリ(irisなど)
  vega_datasets

# ライブラリの書き出し
python -m pip freeze > requirements.txt

# Jupyterlabの起動(ローカルホスト以外にも見えるように)
Jupyter-lab --ip='0.0.0.0' --NotebookApp.token=''
```

### Mac OS / Ubuntu

```bash
# 仮想環境の構築
python3 -m venv .venv

# 仮想環境の起動
source ./.venv/bin/activate

# Install Library
python -m pip \
  
  # Jupyterlab
  install Jupyterlab \
  
  # Jupyterlabの日本語化
  jupyterlab-language-pack-ja-JP \
  
  # 拡張機能を追加する拡張機能
  # jupyter_contrib_nbextensions \
  
  # JupyterlabのGit拡張機能
  jupyterlab-git \
  
  # 変数の確認するための拡張機能
  lckr_jupyterlab_variableinspector \
  
  # Pythonコードのフォーマッター
  jupyterlab-code-formatter \
  
  # コード補完機能
  'jupyterlab>=4.0.0,<5.0.0a0' jupyterlab-lsp \

  # コード自動整形
  # jedi-language-server \
  # 'python-lsp-server[all]' \
  'python-lsp-server[autopep8]' \
  # autopep8 \
  
  # ChatGPTの拡張機能
  # jupyter-ai[all] \
  jupyter-ai langchain-openai
  
  # Data Science
  matplotlib \
  pandas \
  numpy \
  polars \
  plotly \
  seaborn \
  scikit-learn \
  tensorflow[and cuda] \
  pycaret \
  shap \
  
  # vaex: BigData向けのpandasの似たライブラリ
  vaex \
  # altair: データ可視化ライブラリ
  altair \
  # vega_dataset: altairとセットで使われるデータセットがあるライブラリ(irisなど)
  vega_datasets

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
- [Windows ( PowerShell ) で venv メモ](https://gist.github.com/laughk/34e74bfc868c85c7105f54807c29006f)

