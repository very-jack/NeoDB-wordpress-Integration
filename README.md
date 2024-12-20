完整介绍：[WordPress 插件-NeoDB Integration 书影音展示页面](https://anotherdayu.com/2024/6322/)

在 [NeoDB API Developer Console](https://neodb.social/developer/) 中点击`Test Access Token`，并 Generate 一个 NeoDB Bearer Token，示例：`Th2121_qs-8agMAlSrkE_tzBbcvjsdkjtlCtr9QHX321312312Ytzo8_YmOxjxg` 。

在终端（Terminal）或命令提示符（Command Prompt）中输入以下代码，将 YOUR_TOKEN 替换为 NeoDB Bearer Token。

```
curl -H "Authorization: Bearer YOUR_TOKEN" https://neodb.social/api/me
```

然后，在WordPress中安装并激活该插件。  

在 Settings-NeoDB Settings 中输入 NeoDB Bearer Token。  

1.1 - 新增手动更新按钮。
