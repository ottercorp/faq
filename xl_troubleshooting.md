# XIVLauncher FAQ

### Table of Contents
<!-- [How do I disable autologin?](#q-how-do-i-disable-autologin) <br> -->
<!-- [不要用管理云权限运行 XIVLauncher CN](#q-do-not-run-xivlauncher-as-admin) <br> -->
[使用 XIVLauncher, Dalamud 和其中的插件安全吗？](#q-are-xivlauncher-dalamud-and-dalamud-plugins-safe-to-use) <br>
[I get an error saying XIVLauncher failed to check for updates when I open the program](#q-i-get-an-error-saying-xivlauncher-failed-to-check-for-updates-when-i-open-the-program) <br>
[I'm on Linux and I keep getting \"XIVLauncher failed to update\" errors](#q-im-on-linux-and-i-keep-getting-xivlauncher-failed-to-update-errors) <br>
[How come the in-game addon \(Dalamud\) doesn't work and/or plugins don't display?](#q-how-come-the-in-game-addon-dalamud-doesnt-work-andor-plugins-dont-display) <br>
[How do I uninstall XIV Launcher?](#q-how-do-i-uninstall-xiv-launcher) <br>
[How do I fix plugins that rely on Dalamud provided opcodes?](#q-how-do-i-fix-plugins-that-rely-on-dalamud-provided-opcodes) <br>
[How do I whitelist XIVLauncher and Dalamud so my Antivirus leaves them alone](#q-how-do-i-whitelist-xivlauncher-and-dalamud-so-my-antivirus-leaves-them-alone) <br>
[XIV isn't saving my new password / how do I clear my saved password?](#q-xiv-isnt-saving-my-new-password--how-do-i-clear-my-saved-password) <br>
[I think XIVLauncher is giving me a Blue Screen of Death. What information would help narrow this down?](#q-i-think-xivlauncher-is-giving-me-a-blue-screen-of-death-what-information-would-help-narrow-this-down) <br>
[How can I fix crashes on startup?](#q-how-can-i-fix-crashes-on-startup) <br>
[Will plugins/XIVLauncher work on patch day?](#q-will-pluginsxivlauncher-work-on-patch-day) <br>
[Can I log in early with this, before the servers go live?](#q-can-i-login-early-to-titlescreen-before-patch-live) <br>
[XL Environment Variables](#q-xl-environment-variables) <br>
[Outdated Plugins List](#q-outdated-plugins-list) <br>
[The launcher shows a red world icon and an error message when trying to log in, and the official launcher doesn't open](#q-the-launcher-shows-a-red-world-icon-and-an-error-message-when-trying-to-log-in-and-the-official-launcher-doesnt-open) <br>
[The Official Launcher isn't working / XIVLauncher failed to check for updates / Patch files could not be verified](#q-the-official-launcher-isnt-working--xivlauncher-failed-to-check-for-updates--patch-files-could-not-be-verified) <br>
[WTFast Config](#q-wtfast-config) <br>
[NVIDIA Driver issue \(7th of January\)](#q-nvidia-driver-issue-7th-of-january) <br>
[How to set an injection delay in rivaTuner/RTSS](#q-how-to-set-an-injection-delay-in-rivatunerrtss) <br>
[Where can I find my FFXIV Installation?](#q-where-can-i-find-my-ffxiv-installation) <br>
[How do I migrate ffxiv and/or xivlauncher files from an old Wine prefix to a new one? \[Linux\]](#q-how-do-i-migrate-ffxiv-andor-xivlauncher-files-from-an-old-wine-prefix-to-a-new-one-linux) <br>
[How do I migrate ffxiv and\\or xivlauncher files from an old installation to a new one? \[Windows\]](#q-how-do-i-migrate-ffxiv-andor-xivlauncher-files-from-an-old-installation-to-a-new-one-windows) <br>
[Why do people keep asking about Steam so much?](#q-why-do-people-keep-asking-about-steam-so-much) <br>
[Can I repair my FFXIV installation?](#q-can-i-repair-my-ffxiv-installation) <br>
[How do I fix a version check error when trying to update FFXIV?](#q-how-do-i-fix-a-version-check-error-when-trying-to-update-ffxiv) <br>
[How can I stop GShade or ReShade shaders from affecting plugin windows?](#q-how-can-i-stop-gshade-or-reshade-shaders-from-affecting-plugin-windows) <br>
[I updated my game with TexTools mods installed. How do I fix crashes?](#q-i-updated-my-game-with-textools-mods-installed-how-do-i-fix-crashes) <br>
<hr>

<!-- ### Q: How do I disable autologin?
Keep the shift key held down while you open XIVLauncher. Keep it held down until the main window appears.
<hr> -->

<!-- ### Q: 不要用管理员权限运行 XIVLauncher CN
对的，你没有听错！ **请不要用管理员权限运行 XIVLauncher CN。** （除此之外，也请不要以管理员权限手动注入 Dalamud，除非你的游戏是管理员启动的。） You should also never let FFXIV run as admin as it can and __will result in your game configuration data becoming write-protected by your own user__. This can result in you being unable to save character config, hotbars, settings, and take screenshots, with no easy solution beyond trying to fix broken permissions or deleting all config and starting over. (SE does not handle file permissions very well)
<hr> -->

### Q: 使用 XIVLauncher, Dalamud 和其中的插件安全吗？

是的！在 Goatcorp（和 Ottercorp），我们非常重视安全。 使用我们的软件绝不应该让其他玩家可以检测到您正在使用第三方修改。 目前，我们没有理由相信史克威尔艾尼克斯会采取任何措施来检测任何形式的客户端修改。 正如我们所使用的 ReShade/GShade、ACT、Teamcraft 和其他社区项目一样。


#### 一般免责声明
你不应该提及在游戏中使用 XIVLauncher 或插件，就像你不应该承认使用 *任何* 第三方修改一样，因为它在技术上违反最终幻想14的服务条款。我们没有报告用户因使用 XIVLauncher、Dalamud 或其中插件而被封禁的案例，但您仍应谨慎行事。所有官方支持的插件都经过代码审查，以确保它们不会利用游戏或做任何会导致您的游戏客户端向游戏服务器发送无效数据的行为。 __我们不能认可来自第三方插件库的任何非官方插件。您使用第三方插件风险自负。__

此外，XIVLauncher 完全是一个 __用爱发电项目__。我们这样做是因为它对我们来说很有趣，而不是因为我们从中获利。这意味着我们始终尽最大努力做到专业和响应迅速，但这也意味着我们为您提供的一切都是“尽最大努力”的基础 - 维护这样的软件需要大量时间，而我们也是如大家一样的普通人 ：）

如果您对 XIVLauncher、Dalamud 或其中插件有任何疑问，请随时在我们的 [QQ频道](https://qun.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&inviteCode=CZtWN&from=181074&biz=ka&shareSource=5) 中提问。我们是一个主要讲中文的社区，对其他语言的支持可能有限。

#### XIVLauncher 安全细节
以下是有关 XIVLauncher 本身的一些其他详细信息。

1. XIVLauncher 是开源的。 您可以在我们的开源仓库 [XIVLauncher GitHub Repo](https://github.com/ottercorp/FFXIVQuickLauncher/) 中审核代码。
2. XIVLauncher 版本现在直接构建在 GitHub 上，您下载的任何内容都可以确定它来自 GitHub 存储库中列出的开源代码版本。 XIVLauncher 版本检查文件被缓存到私有云存储上，以帮助减少您达到 GitHub API 速率限制和特定国家/地区的 ISP 限制的机会。 文件下载将显示我们的代理域（`ffxiv.wang`），但这会重定向到 GitHub 或中国大陆的 CDN/云存储 （如果需要的话）。 您可以使用您选择的网络分析工具来验证此行为。 代理 使用腾讯云CDN缓存数据，并且只有极少部分开发者可以通过控制台进行访问。
3. 如果 XIVLauncher 已被修改，或者您正在运行用于开发的版本，它将清楚地表明它是调试版本或其他测试/不受支持的版本。 ![unsupported xivlauncher build](images/xivlauncher_unsupported.png).
4. XIVLauncher 使用 Windows 凭据管理器安全地存储您的帐户凭据（包括密码和快速登录凭据）。 您的密码和凭据已加密，只能由授权程序访问。 但是，这确实意味着如果有人设法访问您的计算机，他们可以从技术上提取您的密码与评剧。（但这种情况下您需要优先考虑的或许不只是账号安全的问题。）
5. XIVLauncher 仅与我们的安全代理、GitHub 和最终幻想14官方网站进行通信。
6. XIVLauncher 旨在完全复制与官方启动器相同的登录和授权过程。 已采取措施确保它始终与官方匹配，直至遇到相同的登录问题。 补丁下载是从SE/盛趣提供的启动器的同一个补丁列表中获得的，所有补丁文件在应用之前都经过验证是正确的。

#### Dalamud 安全细节
以下是有关 Dalamud 的一些其他详细信息。

1. Dalamud **是**一个代码注入框架。根据定义，它的外观和行为都类似于病毒程序。您的防病毒软件甚至可能认为它是有害或潜在有害的软件！您可以在常见问题解答的其他地方阅读更多关于 [将 Dalamud 列入白名单](#q-how-do-i-whitelist-xivlauncher-and-dalamud-so-my-antivirus-leaves-them-alone) 的信息。 __我们建议加入白名单以获得最佳体验，但您的电脑环境可能并不需要。__
2. Dalamud 允许您读取游戏内存和网络数据包。 您可以将此行为与使用 ACT 进行类比。
3. Dalamud 框架自带修改游戏内存/Hook游戏客户端内存的能力和插件可以调用的函数。 然而，我们仅在官方 [Dalamud 游戏数据 API](https://goatcorp.github.io/Dalamud/api/index.html) 中提供对游戏数据的只读访问（在适用的情况下）。

#### 插件安全细节
以下是有关 Dalamud 插件的一些其他详细信息。

1. 我们官方插件库中的插件已被我们视为“可以安全使用”。
2. 官方支持的插件应始终从`/xlplugins`插件安装程序直接下载/安装在游戏中。您无需手动下载或手动安装它们。
3. Dalamud 支持第三方插件库，但是支持有限：
- 我们不会为非官方插件提供支持
- 虽然许多非官方插件可以安全使用，但其他插件可能会利用游戏或创建不安全的状态，从而将无效数据发送到游戏服务器从而导致封禁。在使用不受支持的插件之前，请谨慎行事。我们不为第三方插件开发者承担任何责任。
- 不支持的插件的故障排除应提交给插件开发人员或其相关社区。请不要为这些插件在我们的官方频道寻求官方支持，即使它们另外的的支持渠道。

#### 网络安全细节
除了最终幻想14官方网站外，您可能也看到以下列表的网络流量。所有连接都尽可能使用 HTTPS。（Square-Enix 和盛趣很笨，他们的一些服务不使用 HTTPS。我们不喜欢这样，但无法控制它。）

您可以在此处找到我们其他 Web 服务的源代码，国服可能并没有完全使用：<https://github.com/goatcorp/XLWebServices/tree/master/XLWebServices>

1. `ffxiv.wang` - 这是 XIVLauncher CN 背后的私有 VPS，由 XIVLauncher CN 的维护者运行，用于代理和缓存 XIVLauncher 和 Dalamud 检查其版本的一些常用文件。它被用来减少到 GitHub 的网络连接数量，这样用户就不必担心达到速率限制和连接不良/被他们国家的防火墙阻止，然后根据需要将流量引导到 GitHub。 VPS 使用 国内的CDN/云服务 依次缓存数据，并且只有极少部分开发者可以通过控制台进行访问。
2. `github.com`、`raw.githubusercontent.com` 和 `ottercorp.github.io` - 它是 GitHub。你现在正在访问的就是！
3. `act1.ff.sdo.com` - 检查服务器状态的盛趣站点。
<hr>

### Q: I get an error saying XIVLauncher failed to check for updates when I open the program
There are a few different reasons that XIVLauncher will fail to open. Here are a few common ones.

#### XIVLauncher is being blocked by my antivirus/firewall
See the main [Antivirus](#) FAQ post for information on how to whitelist XIVLauncher. 

#### GitHub Rate Limits
If you've made a lot of queries to github recently, it's possible they may have rate-limited you. This is usually a combined effort of XIVLauncher, Dalamud, Dalamud plugin updates, Gshade, etc all being done in rapid succession, which shouldn't happen under normal circumstances.

1. Try to visit <https://api.github.com/rate_limit> and see if the post loads (or downloads a json file)
2. Look for `resources.core.remaining`. If it's 0, you've hit GitHub's rate limit
3. If you've hit the limit, grab the timestamp number from resources.core.reset and convert the UTC timestamp into a human-readable date. <https://www.unixtimestamp.com/> works great for this.
4. Wait the alloted time before launching again, or the timeout period could be extended (if you absolutely need to get in game, use the official launcher during this time)

#### Not sure?
For the fastest support, head over to the XIVLauncher Discord and post into the #xivlauncher-issues channel with the error you're getting, a screenshot (if possible), and your `output.log` file which can be found in `%appdata%\xivlauncher` (Use `f!faq logxl` in the XIVLauncher discord for more details there). 
<hr>

### Q: **I'm on Linux and I keep getting \"XIVLauncher failed to update\" errors**

On some more recent Linux distributions, TLS 1.0 and 1.1 has been disabled. This causes an issue with Wine and FFXIV/XIVLauncher because it may not always negotiate TLS correctly.

You can fix this by setting your `dssenh` DLL override to native if it isn't already. (dssenh=n as an environment variable or in Lutris)

This has also been added to the xivlauncher Lutris script as well.

Thank you to kainz0r for this tip!
![Example](images/LinuxConfigScreenshot.png)

On **Fedora**? You will need to run `sudo update-crypto-policies --set DEFAULT:FEDORA32` in order to lighten up the security policies as Fedora 33 and later have stricter SSL/TLS settings. `FEDORA32` didn't work? Try instead: `sudo update-crypto-policies --set LEGACY`
<hr>

### Q: How come the in-game addon (Dalamud) doesn't work and/or plugins don't display?

Like many other game tools, Dalamud works by injecting into the FFXIV process and hooking DirectX. Occasionally, it conflicts with other tools or can't work because of them.

Some of the more common ones that may cause issues are:
- **Common Third-Party Antivirus** programs. See the dedicated FAQ for this using `f!faq av`
- **FRAPS** please make sure FRAPS is closed when opening FFXIV. It hooks directx for the FPS display and/or recording. You can open it for those features after the game is running.
- **Logitech GHub** We don't know why this is a  problem application, but it is. THis program may cause Dalamud to crash when exiting the game leaving you on a black screen that's stuck and has to be closed uncleanly. 
- **MacType** makes no changes to FFXIV because it doesn't use normal fonts anyways. Block it from hooking to FFXIV and you'll be fine.
- **MSI Afterburner** contains RTSS. See below.
-  **OBS** Some of the streaming modes involve hooking directx for better capture. This can cause plugins to render in streams or to not render at all. You may need to change your capture methods.
- **RivaTuner**/**RTSS** Either blacklist FFXIV from automatic hooking or [set a RTSS load delay](#q-how-to-set-an-an-injection-delay-in-rivatunerrtss). RTSS can be used after Dalamud loads without issues.
- **SpecialK** This also injects into DirectX and can mess things up for Dalamud's injection. It's not consistent, but you probably shouldn't use it unless you have a way of making it hook after Dalamud has loaded.
<hr>

### Q: How do I uninstall XIV Launcher?

You can uninstall XIVLauncher like any normal windows program though the control panel or windows 10 setting app. If you want to purge any trace of it, check for and remove these folders.

Program installation and old versions:
`%localappdata%\XIVLauncher`
`%localappdata%\goatsoft` (if it exists)

Settings/plugins and other user config
`%appdata%\XIVLauncher`
<hr>

### Q: How do I fix plugins that rely on Dalamud provided opcodes?
Certain plugins and features (Universalis updates, PennyPincher, and more), require knowing about the FFXIV client's current opcodes. These change every patch and can sometimes take more time to sort out before a Dalamud update for a new patch is ready.

If you need to refresh your opcode information after it was updated, please relaunch the game. Dalamud will check for updated definitions when it is launched.
<hr>

### Q: How do I whitelist XIVLauncher and Dalamud so my Antivirus leaves them alone?

Please make exceptions (or whitelist) the following folders:
 - `%localappdata%\XIVLauncher`
 - `%appdata%\XIVLauncher`
 - `Your FFXIV game installation folder`

### Please also restart your computer afterwards

#### You may also need to reset Dalamud (the plugin system)
To reset dalamud, remove your `%appdata%\XIVLauncher\addon\Hooks` folder. Or type `f!faq delete dalamud` in the XIVLauncher discord and Franzbot will guide you through.

#### You should also try to whitelist the following files if possible:
1. `<your ffxiv installation>\game\ffxiv_dx11.exe`
**and**
2. `%localappdata%\XIVLauncher\XIVLauncher.exe`
3. `%localappdata%\XIVLauncher\app-X.Y.Z\XIVLauncher.exe` NOTE: replace X.Y.Z with the latest version available. **This changes with every launcher update**
4. `%appdata%\XIVLauncher\addon\Hooks\W.X.Y.Z\Dalamud.Injector.exe` NOTE: replace W.X.Y.Z with the latest version available. **This changes with every dalamud update**
5. `%appdata%\XIVLauncher\addon\Hooks\W.X.Y.Z\Dalamud.dll` NOTE: replace W.X.Y.Z with the latest version available. **This changes with every dalamud update**
6. `%appdata%\XIVLauncher\runtime`

#### Instructions for individual AV

#### Avast:
<https://support.avast.com/en-ww/article/Antivirus-scan-exclusions> <br>

#### AVG:
<https://support.avg.com/SupportArticleView?l=en&urlname=AVG-Antivirus-scan-exclusions> <br>

#### Bitdefender:
<https://www.bitdefender.com/consumer/support/answer/13427/> <br>
**NOTE**: BitDefender users will also need to whitelist xivlauncher's program files (local appdata stuff) through the **[BitDefender firewall](https://www.bitdefender.com/consumer/support/answer/13425/)**. Otherwise, XIVLauncher will fail to check for updates, possibly fail to apply patches, and won't be able to download plugins.

#### Kaspersky Internet Security
<https://usa.kaspersky.com/blog/kaspersky-add-exclusion/11075/> <br>
**NOTE 1**: Please add **file and folder** exclusion in the `Threats and Exclusions` section for the Antivirus component. See the lists above for all details. You may also need to explicitly manager which AV scanners need to be disabled. 


<details>
  <summary>Example screenshot of AV settings</summary>
	
  ![image](https://user-images.githubusercontent.com/10376708/131000436-35097d20-f186-4942-ab43-73e51ff77609.png)
	
</details>

**NOTE 2**: You may need to whitelist xivlauncher's program files in the **[Kaspersky firewall](https://support.kaspersky.com/15163)** Application Rules as well. You'll know if you need to do this if you receive error messages related to checking for updates, applying patches, or downloading plugins and your logs indicate an access permission issue.

#### McAfee:
<https://service.mcafee.com/webcenter/portal/cp/home/articleview?articleId=TS102056> <br>
**NOTE**: McAfee doesn't allow you to whitelist folders. Instead, you'll need to whitelist files, which is more annoying and also version-specific. See the list above.

#### Norton:
<https://support.norton.com/sp/en/us/home/current/solutions/v3672136> <br>
or <https://www.lifewire.com/exclude-files-from-norton-antivirus-scans-153348> <br>
NOTE: You may also need to make exclusions from active detection or another similarly named feature.

#### Windows Defender:
<https://support.microsoft.com/en-us/help/4028485/windows-10-add-an-exclusion-to-windows-security> <br>

(**PLEASE PROCEED WITH CAUTION**. If you're installing dev plugins, third-party plugins, or something outside of the normal /xlplugins method, we cannot be sure that the plugins will work, be undetected in-game, and not cause harm to your computer)
<hr>

### Q: XIV isn't saving my new password / how do I clear my saved password?

XIV Launcher saves user credentials in the Windows Credential Manager. They will be appropriately labelled so you can find the exact one you want to edit/remove.

1. Open the Windows Credential Manager application. The fastest method is to just start typing its name in the start menu.
2. Select button for Windows Credentials
3. Scroll down until you see an entry like FINAL FANTASY XIV-username and expand the entry
4. Delete the entry. XIVLauncher will no longer be able to load it.
5. Now open xivlauncher and try to login.

If you need more help, a basic guide can be found on <https://pureinfotech.com/credential-manager-windows-10/>
<hr>

### Q: I think XIVLauncher is giving me a Blue Screen of Death. What information would help narrow this down?
(NOTE: It's probably not XIV Launcher, but the following information will help us verify that)

1. What stop code are you getting?
2. What is the faulting application or driver?
3. When did this start happening for you?
4. Which plugins do you have installed? Does it still happen if you disable them and selectively re-enable them one by one?
5. Have you done a full uninstall of XIVLauncher and reinstall? (see a few posts above for details)

If unsure about some of those details or if the Windows Event Viewer doesn't tell you, [Bluescreenview](https://www.nirsoft.net/utils/blue_screen_view.html) can read the memory dump (please let the computer finish it without hitting the reset button while it dumps your memory to hard drive)
<hr>

### Q: How can I fix crashes on startup?
Please try to install the VC Redist from Microsoft at <https://github.com/abbodi1406/vcredist/releases/latest>, as well as the .NET 4.8 Runtime <https://dotnet.microsoft.com/download/dotnet-framework/thank-you/net48-web-installer>.
If you are still facing issues, please message us in #xivlauncher_issues
<hr>

### Q: Will plugins/XIVLauncher work on patch day?
Please remember that many of the developers have school/jobs/both and live across a variety of time zones. Things will be updated when they can be. The notion that "XL could be gone at any time" still exists. **We have no clue how much work/time any possible patch may take and we can't give you any ETAs - it's impossible.** Please don't badger us about it, the more support we have to do on patch days, the less work we can do to fix things.

XIVLauncher:
- Users do not need to take any preemptive actions for XIVLauncher compatibility with a new patch.
- Unless SE decides to completely change how authentication or patch download/updating works, the launcher will work just fine on patch days.

Dalamud:
- Dalamud has an internal mechanism that checks the client version and a whitelisted compatibility file.
- If the client version does not match what's whitelisted, Dalamud will not load.
- Once Dalamud has been whitelisted, it will load the next time you launch with XIVLauncher. (We'll also make an announcement on Discord)
- Dalamud may or may not require updates to be made compatible with the current client. This ultimately depends on how much changed internally and we cannot provide any estimates on how long it may take to whitelist as compatible.

Plugins:
- Expect all plugins to stop working every patch.
- Once Dalamud has been whitelisted for a new patch, it will try to load plugins.
- It's entirely possible that a patch will be fine for Dalamud, but break a plugin. (If this happens, you'll want to disable/remove the plugin until it's updated)
<hr>

### Q: CAN I LOGIN EARLY TO TITLESCREEN BEFORE PATCH LIVE????
In theory, yes. But you'll probably have expired authorization and have to login again anyways.

Like every patch maintenance, the lobby server will likely be taken offline as usual. Even assuming you get the patch downloaded and applied mid-maintenance, your authorization will almost assuredly be expired before things are back up.  **Especially for housing patches as SE never ends those early.**

You can make use of XL's "wait for maintenance to be over" features to sit and check for boot patches (no login required) and then prompt you to login for game patches as soon as they are generally available.

The "wait for maintenance to be over" feature can also check for servers to be live every ~15 seconds to get you logged in as soon as things are live.

As with any patch, **in-game addons will be automatically disabled until Dalamud is updated for new patch content**. Do not manually inject Dalamud as a startup application unless you'd like to crash your client  
<hr>

### Q: XL Environment Variables

You can set `XL_PRERELEASE=true` for testing a new release of xivlauncher if applicable.

**If you set this on without knowing what it does, we will not help you if something breaks**

Don't use the wine env var anymore. Just use the properly working Lutris scripts that work with SquirrelSetup.

 **Support will not be provided if you are not on the current version of XL, Dalamud, and plugins. Use with caution as outdated versions will likely crash.**
<hr>

### Q: Outdated Plugins List
Between patches breaking them, time, and/or interest, these plugins are not currently updated and the developers are aware. If you'd like to help maintain a plugin, we can help you find their repo and contact if they're still active.

#### Chat Extender:
Broken in: 5.4
Status: Being split into multiple separate plugins that can be maintained separately. (ChatBubbles and Chat Translator are two of these plugins)
<hr>

### Q: The launcher shows a red world icon and an error message when trying to log in, and the official launcher doesn't open
This is an issue with Square Enix servers that has been affecting players in the US for a while now, being caused by the login servers being hosted directly by SE in Japan and not taking care of their routes to players.

To remedy it, you can either wait a while and try again then, or set your VPN to Japan until you are on the title screen. Then you should be able to play normally without a VPN. DNS changes have also been said to help.

We can recommend mudfish as a VPN for playing FFXIV as it's cheap and seems to work reliably.
If you get errors when patching, we recommend ProtonVPN or CloudFlare with Warp.

To troubleshoot, you can ping frontier.ffxiv.com, SE's Japanese login server.
<hr>

### Q: The Official Launcher isn't working / XIVLauncher failed to check for updates / Patch files could not be verified

Most likely, there's an issue with your network connection or the route it's taken to Square Enix's servers and/or GitHub. The only information XIVLauncher really gets from this is "something went wrong" though.

While this usually is a per-household kinda thing, there's no guarantee that multiple computers in the same location would get load balanced onto the same servers (which is why one computer worked and another didn't). 

If you're sure this isn't a firewall issue or a rate limit, here are some things you can try.

1. Reboot the computer
2. Reboot the network equipment (modem and router)
3. Try different DNS
	- Google offers 8.8.8.8 and 8.8.4.4
	- CloudFlare offers 1.1.1.1 and 1.0.0.1 
	- Level3 offers 4.2.2.2 and 4.2.2.4
4. Try a VPN
	- If you already connect using a VPN, try disconnecting it first
	- If you want to try a free VPN service, CloudFlare offers one at <https://1.1.1.1/> or you can try ProtonVPN for more control.
	- If you want to try a paid VPN service (still no guarantee) we've recommended MudFish in the past.
5. Copy a working FFXIV install from another computer
	- The easiest method is to just copy the folder onto a large flash drive or external HD
	- If you're familiar with setting up Windows Sharing, you can also share the drive/folder from a working computer and copy it over your network

### Q: WTFast Config
![wtfast config settings](images/wtfastconfig.png)
<hr>

### Q: NVIDIA Driver issue (7th of January)
If you experience crashes with the Nvidia driver from the 7th of January, please try rolling back to the last release before the holidays from the 15th of December.

The release from the 7th seemingly introduced a change or bug that will cause FFXIV to crash under certain conditions when XL is loaded.

We are still looking into this.
<hr>

### Q: How to set an injection delay in RivaTuner/RTSS

1. Go to `C:\Program Files (x86)\RivaTuner Statistics Server\Profiles\\`
2. Open the **ffxiv_dx11.exe.cfg** file in your text editor of choice.
3. Find the `[Hooking]` section and change 2 parameters there:
```
InjectionDelay=15000
InjectionDelayTriggers=KERNEL32.dll,USER32.dll
```
If they are not present, add them

<hr>

### Q: Where can I find my FFXIV Installation?
(AKA: What does XIVLauncher mean by GamePath?)

FFXIV installs to a few different locations depending on whether you used the official installer or steam, when you installed it, and potentially if you installed the free trial or not. Here are some of the common paths.

Whatever you do, DO NOT SELECT THE `BOOT` OR `GAME` FOLDER. But if you already have a copy of FFXIV installed, you'll want the folder that contains them.

Official Launcher:
`C:\Program Files (x86)\SquareEnix\FINAL FANTASY XIV - A Realm Reborn`

Steam:
`C:\Program Files (x86)\Steam\steamapps\common\FINAL FANTASY XIV Online`
`C:\Program Files (x86)\Steam\steamapps\common\FINAL FANTASY XIV - A Realm Reborn`
__NOTE__: If your steam library is on another drive, it will have a different, but similar structure. <br>
![Example](images/xivlaunchersSettings.png)
<hr>

### Q: How do I migrate ffxiv and\/or xivlauncher files from an old Wine prefix to a new one? \[Linux\]

Once you've made your new xivlauncher-based prefix, you can copy files from your old ffxiv prefix for the following:

**Copy a FFXIV Install from one prefix to another \(or move/symlink as desired\)**

from:
`~/Games/<old prefix>/drive_c/Program Files (x86)/SquareEnix/FINAL FANTASY XIV - A Realm Reborn`
<br>
to:
`~/Games/<new prefix>/drive_c/Program Files (x86)/SquareEnix/FINAL FANTASY XIV - A Realm Reborn`

**Copy your user/character settings:**

from:
`~/Games/<old prefix>/drive_c/users/<username>/My Documents/My Games/FINAL FANTASY XIV - A Realm Reborn`
<br>
to:
- (Wine 5) `~/Games/<new prefix>/drive_c/users/<username>/My Documents/My Games/FINAL FANTASY XIV - A Realm Reborn`
- (Wine 6) `~/Games/<new prefix>/drive_c/users/<username>/Documents/My Games/FINAL FANTASY XIV - A Realm Reborn`

**Copy XIV Launcher config \(please reinstall plugins\)**:

from:
`~/Games/<old prefix>/drive_c/users/<username>/Application Data/XIVLauncher/pluginConfigs`
<br>
to:
- (Wine 5) `~/Games/<new prefix>/drive_c/users/<username>/Application Data/XIVLauncher/pluginConfigs`
- (Wine 6) `~/Games/<new prefix>/drive_c/users/<username>/AppData/Roaming/XIVLauncher/pluginConfigs`
<hr>

### Q: **How do I migrate ffxiv and\/or xivlauncher files from an old installation to a new one? \[Windows\]**

**Copy a FFXIV Install**
For the most part, FFXIV is portable. You just need to make sure you've installed DirectX as needed. I recommend installing the launcher with SE's installer first, and then replacing the files with a backup if you don't want to patch.
__NOTE__: You shouldn't do this if you had Textools installed. Or at least, make sure to restore indexes first as it probably broke your client.

**Copy your user\character settings:**
`%USERPROFILE%\Documents\My Games\FINAL FANTASY XIV - A Realm Reborn`

**Copy XIV Launcher config (please reinstall plugins)**:
__NOTE__: do not copy other config or folders as those are unique to that particular computer. You should set them up per machine.
`%appdata%\XIVLauncher\pluginConfigs`
<hr>

### Q: Why do people keep asking about Steam so much?
Steam Integration = "I want the steam program to see I'm playing FFXIV and do the overlay thing"

Use Steam service account = "I bought FFXIV through Steam, which is not the same as the Windows platform."

#### How to override your FFXIV steam entry to open XIVLauncher instead
1. Right Click on your game
2. Go to Properties
3. Set Launch Options...<br>Set the launch option to `"C:\Users\YOUR_USERNAME_HERE\AppData\Local\XIVLauncher\XIVLauncher.exe" %command%` (the quotes are important). If you're one of those monsters with your userprofile in a nonstandard location, you will be expected to adjust the full path accordingly.
<hr>

### Q: Can I repair my FFXIV installation?

Short answer: No, not without reinstalling the game.

#### General steps  to reinstall the entire game
1. Go to your ffxiv installation folder (refer to your gamepath)
2. Delete the `boot` and `game` folders
3. Open xivlauncher and login. It should ask to patch

Fun answer: XIVLauncher can assist you in selectively reinstalling only certain portions of the FFXIV game client if needed. Or the entire game.

#### General steps to reinstall just ARR:

1. Go to your ffxiv installation folder (refer to your gamepath)
2. Go to the `game` folder
3. Select all the files except the `sqpack` folder
4. If you have reshade/reshade, unselect those files to preserve them (gshade-presets, gshade-shaders, GShade.ini, dxgi/d3d11)
5. Delete the selected files so only the sqpack folder remains (and reshade/gshade files if applicable)
6. Go to the `sqpack` folder now
7. Delete the `ffxiv` folder there
8. Open xivlauncher and login. It should ask to patch

#### General steps to reinstall one or more expansions:
1. Go to your ffxiv installation folder (refer to your gamepath)
2. Go to the `game` folder
3. Go to the `sqpack` folder now
4. Delete the corresponding expac folder[s] you want to reinstall.
    4a. ex1 = heavensward
	4b. ex2 = stormblood
	4c. ex3 = shadowbringers
5. Open xivlauncher and login. It should ask to patch

<hr>

### Q: How do I fix a version check error when trying to update FFXIV?
1. Go to `<your user folder>\Documents\My Games\FINAL FANTASY XIV - A Realm Reborn`
2. Open the `FFXIV_BOOT.cfg` file in your text editor of choice.
3. Change `BootVersionCheckMode` to `1`
4. Relaunch.

<hr>

### Q: How can I stop GShade or ReShade shaders from affecting plugin windows?
1. Go to `<your game installation folder>\FINAL FANTASY XIV - A Realm Reborn\game`
2. Make sure the game is closed
3. If there is a file called `d3d11.dll` or `dinput8.dll` **rename it** to `dxgi.dll`
4. Relaunch.

<hr>

### Q: I updated my game with TexTools mods installed. How do I fix crashes?
You'll know if you're affected by this because the official launcher will crash the game too. This issue is not caused by XIVLauncher.

While the last few game patches have been relatively fine to keep your Textools mods enabled as it will do minor adjustments to fix things up, please refer to the Textools Discord for best practices.

To fix the crash, open Textools, click on the Help menu, and select "Download Index Backups" and then "Start Over" to repair files broken from updating with Textools modifications.
<hr>

Want to add a new FAQ entry? Please use the template below and PR to the main [FAQ repo](https://github.com/goatcorp/faq)
```
### Basic Title
FAQ content
<hr>
```
Then add it to the Table of Contents using `[Name / Title here](#anchor here) <br>`

[Return to the top](#table-of-contents)<br>
[Return to the main Readme](https://goatcorp.github.io/faq)
