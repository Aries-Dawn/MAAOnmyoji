<!-- markdownlint-disable MD033 MD041 -->
<p align="center">
  <img alt="LOGO" src="doc\doc_img\应声虫.png" width="256" height="256" />
</p>

<div align="center">

# MAAOnmyoji

</div>

基于 [MaaFramework](https://github.com/MaaXYZ/MaaFramework) 的痒痒鼠每日任务代理。

> **MaaFramework** 是基于图像识别技术、运用 [MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights) 开发经验去芜存菁、完全重写的新一代自动化黑盒测试框架。
> 低代码的同时仍拥有高扩展性，旨在打造一款丰富、领先、且实用的开源库，助力开发者轻松编写出更好的黑盒测试程序，并推广普及。

## 功能列表以及

- [x] 每日主界面奖励领取
- [x] 自动地鬼（2普通+1悬赏）
- [ ] 自动逢魔+极
- [ ] 自动阴界之门
- [ ] 自动悬赏封印
- [ ] 任务结束后领取花合战
- [ ] 任务结束后领取花车


## 如何开发

0. 使用右上角 `Use this template` - `Create a new repository` 来基于本模板创建您自己的项目。

1. 完整克隆本项目及子项目（地址请修改为您基于本模板创建的新项目地址）。

    ```bash
    git clone --recursive https://github.com/MaaXYZ/MaaPracticeBoilerplate.git
    ```

    **请注意，一定要完整克隆子项目，不要漏了 `--recursive`，也不要下载 zip 包！** 这步未正确操作会导致所有 OCR（文字识别）失败！

2. 下载 MaaFramework 的 [Release 包](https://github.com/MaaXYZ/MaaFramework/releases)，解压到 `deps` 文件夹中。

3. 配置资源文件。

    ```bash
    python ./configure.py
    ```

4. 按需求修改 `assets` 中的资源文件，请参考 MaaFramework 相关文档。

    - 可使用 [MaaDebugger](https://github.com/MaaXYZ/MaaDebugger) 进行调试；
    - 也可以在本地安装后测试：

        1. 执行安装脚本

            ```bash
            python ./install.py
            ```

        2. 运行 `install/MaaPiCli.exe`

5. 完成开发工作后，上传您的代码并发布版本。

    ```bash
    # 配置 git 信息（仅第一次需要，后续不用再配置）
    git config user.name "您的 GitHub 昵称"
    git config user.email "您的 GitHub 邮箱"
    
    # 提交修改
    git add .
    git commit -m "XX 新功能"
    git push origin HEAD -u
    ```

6. 发布您的版本

    需要先修改仓库设置 `Settings` - `Actions` - `General` - `Read and write permissions` - `Save`

    ```bash
    # CI 检测到 tag 会自动进行发版
    git tag v1.0.0
    git push origin v1.0.0
    ```


## 鸣谢

本项目由 **[MaaFramework](https://github.com/MaaXYZ/MaaFramework)** 强力驱动！图形界面由 **[MFAWPF](https://github.com/SweetSmellFox/MFAWPF)** 提供。

<!--

感谢以下开发者对本项目作出的贡献（下面链接改成你自己的项目地址）:

<a href="https://github.com/Aries-Dawn/MAAOnmyoji/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Aries-Dawn/MAAOnmyoji&max=1000" />
</a>

-->