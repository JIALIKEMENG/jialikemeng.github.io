**使用方法：**

- 对您的数据进行适当的备份；
- 在智能手机上启用开发人员选项；
- 从开发人员面板打开USB调试；
- 在设置中，断开与任何 OEM 帐户的连接（删除 OEM 帐户包时，它可能会将你锁定在锁屏界面上，因为手机无法再关联你的身份）；
- 安装 ADB：
> 1. 下载[Android平台工具](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)或[蓝奏云下载](https://www.lanzv.com/igjwS1nd1xmj)并将其解压缩到某个地方；
> 2. 将 android 平台工具[添加到您的 PATH](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/) 中，或者确保从同一目录启动 UAD-ng；
> 3. 为您的设备安装 [USB 驱动程序](https://developer.android.com/studio/run/oem-usb#Drivers)。三星手机在安装PC端Samsung Dex时自动安装了驱动，因此无需下载；
> 4. 检查您的设备是否被检测到： adb devices
- 在[此处](https://github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation/releases)下载适用于您的操作系统的最新版本的 UAD-ng。仅当默认版本（带有 Vulkan 后端）未启动时，才使用该版本。

注意：
中国手机用户可能需要使用AOSP列表来删除一些库存应用程序，因为这些中国制造商（尤其是小米和华为）一直在使用AOSP软件包的名称用于他们自己的（修改和闭源）应用程序。
重要提示：
每当您的 OEM 向您的手机推送更新时，您都必须运行此软件，因为某些未卸载的系统应用程序可能会重新安装。

[Windows ADB客户端方法](https://github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation)
[常见问题解答](https://github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation/wiki/FAQ)
