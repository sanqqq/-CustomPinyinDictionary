# 自建拼音输入法词库

> 目前提供 <u>Fcitx 5</u> (Linux / Android) 以及 <u>Gboard</u> (Android + Magisk) 两种词库数据格式。

当前词库，包含了以下内容：

   * 常见的成语、俗语、诗歌等
   * 中华人民共和国四级行政区划名称（感谢[Administrative-divisions-of-China](https://github.com/modood/Administrative-divisions-of-China)）
   * 世界各个国家国名全称、简称（感谢[wgii](https://github.com/occultskyrong/wgii))
   * 世界各国和地区名称及一级行政区划（数据来源：中华人民共和国海关总署)
   * 常见人名
   * 网络提供的第三方输入法词库
   * ……

已对以上所有数据进行去重、精简处理，最终词汇量等信息详见 [Releases](https://github.com/wuhgit/CustomPinyinDictionary/releases)。


---

<div>
	<img src="https://fcitx-im.org/fcitx.png" alt="Fcitx5 logo" width="100">
</div>

# Fcitx 5

下载 `CustomPinyinDictionary_Fcitx_<版本号>.zip` 并解压，得到词库文件 `CustomPinyinDictionary_Fcitx.dict`

- Linux

	将词库文件复制粘贴到目录 `~/.local/share/fcitx5/pinyin/dictionaries/` 中（如果没有这个目录，您可以自行创建），重启 <u>Fcitx</u> 后即可生效。

- Android

	拼音输入模式下，在输入法键盘上选择 `输入法设置 > 词典`，添加词库文件即可。


---


<div>
	<img src="https://play-lh.googleusercontent.com/X64En0aW6jkvDnd5kr16u-YuUsoJ1W2cBzJab3CQ5lObLeQ3T61DpB7AwIoZ7uqgCn4=s180" alt="Gboard logo" width="100">
</div>

# Gboard (Magisk module)

> 🔴 注意！
> - 本词库仅对 ___中文（简体） 拼音___ 的键盘语言和布局生效，请检查 Gboard 相关设置。
> - 如果是旧版数据用户 (即 2022-04-22 前通过直接替换文件方式进行安装的用户) ，先恢复词库至您之前备份的数据，若没有相应备份，当迁移至 Magisk 模式时，请先在模块安装时选择卸载，此时模块会将原有词库替换为空白数据，随后再进行安装。

安装、升级、卸载此模块均 **不需要重启**，即时生效。

## **使用方法**

- 首次安装
   1. 下载 `CustomPinyinDictionary_Gboard_Magisk_<版本号>.zip`。
   2. 使用 Magisk 应用 `从本地安装`，选择之前下载的文件。
   3. 使用音量键选择`安装`。

- 升级
   - 直接通过 Magisk 应用进行检查更新并安装。

- 卸载
   1. 参考`首次安装`的 1～2 。
   2. 使用音量键选择`卸载`。
   3. 在 Magisk 模块管理页面对本模块进行 `移除`。


   > 若忘记执行卸载直接移除，可以再重新执行一遍卸载流程，过程中选择卸载，随后移除模块即可。


## **注意**

词库导入后，可能需要一点时间后才能在输入时感知到新词。
  
> 您可以在 `Gboard 设置 > 字典 > 个人字典 > 中文（简体）` 查看到导入后本词库的数据。

为获得更好的使用体验，建议对 <u>Gboard</u> 中以下设置进行修改：

`Gboard 设置 > 高级 > 学习`

  - 关闭 **个性化设置**
  - 关闭 **改进语音和输入功能，让所有用户受益**
