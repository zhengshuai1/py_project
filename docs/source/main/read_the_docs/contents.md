# Sphinx + Read the Docs文档构建

## 执行 sphinx-quickstart 构建项目框架

## 主题设置
``` 
html_theme = 'sphinx_rtd_theme'
```

## markdown支持
```
extensions = [
    'recommonmark',
    'sphinx_markdown_tables'
] 
```

## 增加edit on github链接
``` 
rst_prolog = """
:github_url: https://github.com/xxx
"""
```