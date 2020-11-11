# 开放 API 文档

[![构建状态](https://codingcorp.coding.net/badges/coding-help-generator/job/54361/build.svg)](https://codingcorp.coding.net/p/api-test-go/ci/job)

本仓库是对外开放 API 文档的管理中心。所有的文档内容皆位于 api.json 文件中，配合可视化编辑器 [Stoplight Studio](https://stoplight.io/studio/) 加持续集成完成文档更新。

## 目录结构

```text
├── Jenkinsfile
├── api.json # 文档内容
├── README.md
```

## API 文档更新指南

下载 [Stoplight Studio](https://stoplight.io/studio/) 后，导入本仓库地址。

![](https://help-assets.codehub.cn/enterprise/20201109151348.png)

通过该软件就可以完成对 API 文档的可视化编辑。

![](https://help-assets.codehub.cn/enterprise/20201109151439.png)

编辑完成后通过该软件新建分支后提交。

![](https://help-assets.codehub.cn/enterprise/20201109152004.png)

### 验证线上内容

链接：https://open-api1-codingcorp.doc.coding.io

一经提交，便会自动触发持续集成任务。
