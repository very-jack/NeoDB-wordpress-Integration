完整介绍：[WordPress 插件-NeoDB Integration 书影音展示页面](https://anotherdayu.com/2024/6322/)

在 [NeoDB API Developer Console](https://neodb.social/developer/) 中点击`Test Access Token`，并 Generate 一个 NeoDB Bearer Token，示例：`Th2121_qs-8agMAlSrkE_tzBbcvjsdkjtlCtr9QHX321312312Ytzo8_YmOxjxg` 。

在终端（Terminal）或命令提示符（Command Prompt）中输入以下代码，将 YOUR_TOKEN 替换为 NeoDB Bearer Token。

```
curl -H "Authorization: Bearer YOUR_TOKEN" https://neodb.social/api/me
```

然后，在WordPress中安装并激活该插件。  

在 Settings-NeoDB Settings 中输入 NeoDB Bearer Token。  

1.1 - 新增手动更新按钮。

参考资料：
hcplantern 的 将 NeoDB 记录整合到 Hugo 中 

1.2 
* 短代码修改为了 [neodb_page]，无需输入其他参数。
* 修改了样式，改为了垂直排布，并且适配了手机。
* 顶部添加类型按钮，现在可以直接选择。
* 底部添加“加载更多”按钮，从而获取更多信息。（之前默认只获取第一页信息）
* 后台设置里添加自定义颜色，可以调整字体颜色和悬停时颜色，以便更好适配自己的主题。
* 后台添加启用分类的按钮，根据需求选择需要展示的类别。
* 现在可以直接将图片缓存到插件目录下的 cache 文件夹中，这样可以规避大陆地区无法获取图片的问题
* 后台“手动更新数据”按钮添加清理图片缓存的功能（默认30天自动清理一次图片缓存）。
