# github actions自动发布PyPI
本action在每次release发布时，自动publish package到PyPI.
## 添加 Actions

添加 Publish Python Package Action，并提交。

## 创建 Secrets
使用TOKEN发布pypi, 前往项目的设置中，添加名称为 PYPI_API_TOKEN 值为 TOKEN 的秘钥，用于上传。