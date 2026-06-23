# MiniLink iOS 技术支持与使用说明

MiniLink 可以将 iPhone 或 iPad 作为蓝牙键盘使用，连接到 Mac、iPad、Android 平板或其他支持蓝牙键盘输入的设备。本文只说明日常使用和排查方法，不涉及软件架构。

技术支持邮箱：prsiancat_6@icloud.com

## 使用前准备

1. 在 iPhone 或 iPad 上打开 MiniLink。
2. 允许 App 使用蓝牙权限。
3. 保持 MiniLink 在前台运行。
4. 在需要输入的目标设备上打开蓝牙设置。

建议首次连接时，让 iPhone/iPad 与目标设备保持在 1 米内，并关闭目标设备上不需要的旧蓝牙键盘连接。

## 连接蓝牙键盘

1. 在 iPhone 或 iPad 上打开 MiniLink。
2. 在目标设备的蓝牙设置中搜索蓝牙设备。
3. 找到并连接 `MiniLink HID`。
4. 回到 MiniLink，确认连接状态显示为已连接。
5. 点击屏幕键盘按键，或发送测试文本，确认目标设备可以收到输入。

![MiniLink 键盘界面](../AppStoreAssets/screenshots/iphone-01-keyboard.png)

## 蓝牙 HID 状态

MiniLink 使用 BLE HID 键盘方式工作。目标设备连接成功后，会把 MiniLink 识别为一个蓝牙键盘，而不是普通文件传输设备。

在部分系统中，蓝牙设置页面可能显示 iPhone 的设备名称，而不是直接显示 `MiniLink HID`。只要 MiniLink 内显示已连接，并且目标设备可以收到输入，即表示连接正常。

![蓝牙 HID 连接状态](../AppStoreAssets/screenshots/iphone-02-ble-hid.png)

## 切换输入设备

如果你连接过多个目标设备，可以在 MiniLink 中切换当前输出目标。切换后，键盘输入会发送到当前选中的设备。

操作建议：

1. 先确认多个目标设备都曾连接过 MiniLink。
2. 在 MiniLink 中选择要输入的设备。
3. 在目标设备上打开任意文本输入框。
4. 点击 MiniLink 键盘，确认输入发送到正确设备。

![切换输出设备](../AppStoreAssets/screenshots/iphone-03-switch-host.png)

## iPad 使用

iPad 版本提供更大的键盘区域，适合横屏输入和桌面使用。连接方式与 iPhone 相同：先打开 MiniLink，再在目标设备蓝牙设置中连接 `MiniLink HID`。

![iPad 键盘界面](../AppStoreAssets/screenshots/ipad-01-keyboard.png)

## 旧设备兼容模式

如果旧 iPad 或部分 Android 设备可以发现 MiniLink，但连接后没有输入反应，可以尝试：

1. 打开 MiniLink 的旧设备兼容模式。
2. 删除目标设备蓝牙设置中保存过的 MiniLink 或 iPhone 记录。
3. 关闭并重新打开目标设备蓝牙。
4. 重新打开 MiniLink，再次连接 `MiniLink HID`。

![旧设备兼容模式](../AppStoreAssets/screenshots/ipad-03-compat.png)

## 常见问题

### 目标设备搜索不到 MiniLink HID

请确认：

1. MiniLink 正在前台运行。
2. iPhone 或 iPad 的蓝牙已经开启。
3. 系统已经允许 MiniLink 使用蓝牙。
4. 目标设备没有连接过太多旧蓝牙键盘。
5. 尝试关闭目标设备蓝牙后重新打开。

### 显示已连接，但无法输入

请尝试：

1. 在目标设备上点击一个可输入文本的位置。
2. 在 MiniLink 中发送测试文本。
3. 断开蓝牙后重新连接。
4. 删除目标设备中保存的 MiniLink 或 iPhone 蓝牙记录后重新配对。
5. 对旧 iPad 或部分 Android 设备启用旧设备兼容模式。

### 蓝牙设置里显示的是 iPhone 名称

这是部分系统的显示方式。只要 MiniLink 内显示连接成功，并且目标设备可以收到键盘输入，就可以正常使用。

### 多设备切换后输入到了错误设备

请在 MiniLink 中重新选择输出目标，并确认目标设备当前处于已连接状态。如果仍然异常，请断开不需要输入的设备后再测试。

## 联系支持

如果问题仍然存在，请发送邮件到：

prsiancat_6@icloud.com

邮件中建议包含：

1. iPhone 或 iPad 型号。
2. iOS 或 iPadOS 版本。
3. 目标设备型号。
4. 目标设备系统版本。
5. 问题现象，例如无法搜索、无法连接、已连接但无法输入。
6. 如方便，请附上蓝牙设置页面和 MiniLink 连接状态截图。
