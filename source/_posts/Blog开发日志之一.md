---
title: Blog开发日志之一
date: 2019-07-23 16:18:00
tags: [Blog开发日志]
---

第一次更换Theme中学到的经验：

1）Gitbub库中的子模块(submodule)貌似不能直接通过pull request的方式分享给其他用户。如果需要该模块，必须单独clone。子模块从其他开发者的库中直接clone而来。可能由于GitHub的防盗版功能，其分享受限制；

2）子模块中的.git文件夹最好删除，不然可能会出现上传错误的可能。.git文件夹包含GitHub的仓库与本地的连接信息。由于子模块由其他用户开发，可能无法直接上传至自己的仓库。建议使用cmd输入命令删除：
```
$ del /F /Q /A /S .git
```

3）Hexo自带的deploy功能使得我们无需使用GitHub的四连上传，生成的网页文件会自动更新到GitHub的仓库。上传到哪一个仓库可通过_config.yml中的deploy修改。


by 猪猪
