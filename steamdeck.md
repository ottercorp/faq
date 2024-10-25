# XIVLauncherCN Linux 安装指南

Linux 版 XIVLauncherCN 以多种不同格式发布，具体取决于您的系统设置。请阅读以下内容，了解为您的系统安装 XIVLauncherCN 的推荐方法：

- **我正在使用带有 Steam 大屏幕的 Steamdeck/Linux 手持设备（无论您是否在 Steam 上拥有 FFXIV）**：您应该遵循 [安装为兼容工具指南](#安装-xivlaunchercn-为兼容工具).
- **我正在使用桌面 Linux 发行版并通过 Steam 拥有 FFXIV**: 您应该遵循 [安装为兼容工具指南](#安装-xivlaunchercn-为兼容工具).
- **我使用的是桌面 Linux 发行版，但未通过 Steam 购买 FFXIV**: 您应该遵循 [作为 Flatpak 或系统包安装指南](#安装-xivlaunchercn-作为-flatpak-或系统包)
- **我正在使用此处未列出的设置**: 您的设置可能不支持 XIVLauncherCN，但仍可以参考 [作为 Flatpak 或系统包安装指南](#安装-xivlaunchercn-作为-flatpak-或系统包) 来进一步确定.

## 安装 XIVLauncherCN 为兼容工具

XIVLauncherCN Steam 兼容工具由名为 [XLM](https://github.com/Blooym/XLM) 的项目负责。所有主要系统配置均提供自动安装脚本，可为您完成大部分设置工作 *（但是，如果您的系统配置未在此处介绍，您可以随时从 [GitHub 发布页面](https://github.com/Blooym/xlm/releases/latest) 手动下载 XLM 二进制文件并以此方式安装）*。

*兼容工具的安装与运行均需要访问 Github，请确保您能够正常与 Github API 进行通信。*

Steam 兼容工具的自动安装程序适用于 Steam 的 `Steam Deck`、`Flatpak` 和 `Native` 软件包。只需将下面适用于您系统的脚本复制并粘贴到终端中，兼容工具就会为您安装。之后，按照以下步骤开始使用它。

**Steamdeck 安装脚本**:

```sh
sh -c "$(curl -fsSL https://file.bluefissure.com/d/FFXIV/Dalamud/xlcore/xlm/install-steamdeck-cn.sh)"
```

**Steam 安装脚本 (Native)**
```sh
sh -c "$(curl -fsSL https://file.bluefissure.com/d/FFXIV/Dalamud/xlcore/xlm/install-native-cn.sh)"
```

**Steam 安装脚本 (Snap)**
```sh
sh -c "$(curl -fsSL https://file.bluefissure.com/d/FFXIV/Dalamud/xlcore/xlm/install-snap-cn.sh)"
```

**Steam 安装脚本 (Flatpak)**
```sh
sh -c "$(curl -fsSL https://file.bluefissure.com/d/FFXIV/Dalamud/xlcore/xlm/install-flatpak-cn.sh)"
```

安装程序完成后，请按照以下步骤使用兼容工具：
- 切换回游戏模式（如果在 Steam Deck 上）或重新启动 Steam 客户端。
- 如果您正在通过免费试用版玩游戏或没有 FFXIV 的 Steam 版本，请导航到您的库并选择“FINAL FANTASY XIV Online”或“FINAL FANTASY XIV Online 免费试用版”。
- 如果您所在的商店中这两款游戏已下架，您可以夺舍大部分没有反作弊的单机游戏进行启动 XIVLauncher.Core，请注意游戏时间会一并算入对应游戏中。
- 打开游戏属性菜单并切换到“兼容性”选项卡。
- 启用“强制使用特定的 Steam Play 兼容工具”复选框。
- 从出现的框中选择“XLCore [XLM]”（如果没有显示，请确保您正确重新启动了 Steam）。
- 您现在可以像往常一样启动游戏。XIVLauncher 将自动安装并为您运行。

## 安装 XIVLauncherCN 作为 flatpak 或系统包

### Flatpak

首先，通过运行 `flatpak remotes` 检查 flathub 是否已安装。如果您没有看到 flathub 的条目，请查看 [https://flathub.org/setup](https://flathub.org/setup) 以获取有关如何安装它的说明。

#### 通过终端

要使用终端将 XIVLauncherCN 安装为 flatpak，请以普通用户身份（无需`sudo`）运行命令 `flatpak install flathub cn.ottercorp.xivlaunchercn`。

#### 通过软件商店 (GNOME/KDE)

某些桌面环境为 Flatpak 存储库提供图形前端，允许您浏览应用商店以更直观的方式安装 Flatpaks。

- 如果您使用的是 GNOME，请打开软件，然后搜索“XIVLauncherCN”。单击结果中的 XIVLauncherCN 条目。单击“安装”。

- 如果您使用的是 KDE，请打开 Discover，然后搜索“XIVLauncherCN”。单击结果中的 XIVLauncherCN 条目。单击“安装”。

其他桌面环境可能在其自己的 Flatpak 前端应用程序中提供 XIVLauncherCN，也可能不提供。如果 XIVLauncherCN 没有出现在 GNOME 软件或 KDE Discover 中，请验证 Flatpak 是否已安装并正在运行，并验证您是否已启用 Flathub 存储库。

#### 将 FFXIV 安装到外部驱动器

如果您想将最终幻想14安装到默认文件夹 (`~/.xlcore_cn/ffxiv`) 之外的任何文件夹，您还需要 Discover Store 中的 `Flatseal`。

运行 Flatseal。在左侧，向下滚动到 XIVLauncherCN。在窗口的主要部分，向下滚动到 `Filesystem`。单击其他文件旁边的文件夹图标。输入您想要安装最终幻想14的路径。

### 系统包

可在[此处](https://github.com/ottercorp/XIVLauncher.Core?tab=readme-ov-file#%E5%88%86%E5%8F%91)找到替代包的列表。请注意，除了兼容工具和 Flatpak 外，其余的都由社区成员维护，并被视为非官方。但是，只要包是最新的，您仍将获得社区支持。

## 常见问题

### Q: 我是 WeGame 端，如何登陆？

暂时不支持 WeGame 端账号登陆。

### Q: 我的配置文件保存在哪里？

配置文件保存到 `~/.xlcore`，除非使用 flatpak 安装运行的 Steam，此时配置文件保存到 `~/.var/app/com.valvesoftware.Steam/.xlcore`。

### Q: 游戏随机消失，休眠后无法恢复

请确保 Steam 商店的 [FINAL FANTASY XIV Online](https://store.steampowered.com/app/39210/FINAL_FANTASY_XIV_Online/) 或 [FINAL FANTASY XIV Online Free Trial](https://store.steampowered.com/app/312060/FINAL_FANTASY_XIV_Online_Free_Trial/) 或其他用于启动 XIVLauncher.Core 的游戏已安装在您的 Steam Deck 的 **内部存储器** 中。

### Q: FINAL FANTASY XIV Online (或 Free Trial) 已在所在的 Steam 商店下架

您可以：
- 打开 `~/.xlcore_cn/launcher.ini` 并将 `IsIgnoringSteam` 设置为 `true`。
- 添加 `XL_APPID=2805730` 到运行命令的最前强制指定使用 Proton 9.0 来运行。
- 如果您将 XIVLauncherCN 安装为兼容工具（XLM）：您可以使用其他任意没有反作弊（会影响 Dalamud 注入）的游戏，将其兼容工具强制设定为 XLM。

### Q: 我的音频有爆裂声/失真

尝试将 “PULSE_LATENCY_MSEC=60” 添加到 Steam 启动选项的开头。

### Q: 我无法控制我的游戏

请在 Steam 中更改 “FINAL FANTASY XIV Online Free Trial” 或 “Proton 9.0” 的控制器布局，**而不是** 更改 XIVLauncherCN 的控制器布局。

如果这不能解决问题，请将 ~/.xlcore_cn/ffxivConfig/FFXIV.cfg 重命名为 FFXIV.cfg.bak，然后从游戏模式再次运行游戏。这会将所有最终幻想14系统设置重置为默认设置。将 FFXIV.cfg.bak 重命名回 FFXIV.cfg 将恢复这些设置。

### Q: XIVLauncher 在尝试通过 Steam 运行时立即关闭

不要在 Steam 中为 XIVLauncher 设置兼容模式。 XIVLauncher 是一个不需要 Proton 运行的原生 Steam 应用程序。

### Q: 我无法输入我的用户名/密码

由于 Steam 文本输入 API 的限制，请使用 Steam Deck 的游戏模式完成输入。

### Q: 我在设置界面的文本框只能够输入，无法删除已有的内容

由于 Steam 文本输入 API 的 BUG，请选中内容高亮后进行输入替换。


[返回顶部](#安装)\
<a href="{{ site.github.baseurl }}/">返回 FAQ 主页</a>
