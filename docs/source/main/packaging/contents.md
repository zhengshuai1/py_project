# Python打包 & 发布到PyPI

按照[官方教程](https://packaging.python.org/en/latest/tutorials/packaging-projects/)操作。

```
packaging_tutorial/
├── LICENSE
├── pyproject.toml
├── README.md
├── src/
│   └── example_package_YOUR_USERNAME_HERE/
│       ├── __init__.py
│       └── example.py
└── tests/
```

## 自动化package版本

使用[setuptools-scm](https://pypi.org/project/setuptools-scm/)自动化设置version。

### 设置pyproject.toml

```
# pyproject.toml
[build-system]
requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
```

```
# pyproject.toml
[project]
# version = "0.0.1"  # Remove any existing version parameter.
dynamic = ["version"]
```
``` 
# pyproject.toml
[tool.setuptools_scm]
write_to = "pkg/_version.py"
```