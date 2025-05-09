# notebook

The Directory of Jupyter Notebook Files

## Notebook to Python Script

Jupyter Notebookを、Python Scriptに変更するコマンド

```powershell
# Jupyter Notebookを、Python Scriptに変換するコマンド
jupyter nbconvert --to script notebook.ipynb

# タグで不要なセルを削除して、Python Scriptに変換するコマンド
# https://nbconvert.readthedocs.io/en/latest/removing_cells.html
jupyter nbconvert --to script notebook.ipynb \
  --TagRemovePreprocessor.enabled=True \
  --TagRemovePreprocessor.remove_cell_tags remove_cell
```
