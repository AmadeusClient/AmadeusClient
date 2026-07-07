# Amadeus Client

高性能 Minecraft 客户端 · 模块化架构 · 内置 GraalJS 脚本引擎

---

## 简介

Amadeus 是一款为 **PVP** 与 **实用功能** 而生的 Minecraft 客户端。采用模块化设计，内置 **GraalJS** 脚本引擎，支持 JavaScript 扩展，轻量高效，高度可定制。

- **官网**：https://amadeusclient.github.io  
- **API 文档**：https://amadeusclient.github.io/api.html  
- **下载**：https://github.com/AmadeusClient/AmadeusClient/releases

---

## 核心特性

- **极致性能** – ASM 字节码优化，极低资源占用
- **模块化设计** – 60+ 独立模块，六大分类，按需开关
- **脚本扩展** – GraalJS 引擎，热重载，无需重启
- **动态 HUD** – 完全拖拽式布局，自由定制
- **丰富设置** – 每个模块独立设置面板
- **安全稳定** – 严格沙箱，上下文隔离

---

## 安装

### 环境要求
- Minecraft 1.20.4
- Java 17+
- Forge 47.x+ 或 Fabric 0.15+

### 步骤
1. 从 [Releases](https://github.com/AmadeusClient/AmadeusClient/releases) 下载最新 `.jar`
2. 放入 `.minecraft/mods/` 目录
3. 启动游戏，按 `RSHIFT` 或 `F6` 打开 ClickGUI

---

## 快速开始

| 操作 | 按键 |
|------|------|
| 打开 ClickGUI | `RSHIFT` / `F6` |
| HUD 编辑模式 | `Ctrl + H` |
| 模块绑键 | ClickGUI 中点击绑定区域 |

### 常用命令

| 命令 | 说明 |
|------|------|
| `.clickgui` | 打开 ClickGUI |
| `.hud` | 打开 HUD 编辑器 |
| `.script load <文件名>` | 加载脚本 |
| `.script reload <脚本名>` | 热重载脚本 |
| `.script reloadall` | 重载所有脚本 |
| `.script list` | 列出已加载脚本 |
| `.vclip <距离>` | 垂直传送 |
| `.hclip <距离>` | 水平传送 |
| `.friend add/remove <玩家>` | 管理好友 |
| `.panic` | 紧急禁用所有模块 |
| `.config save <名称>` | 保存配置 |
| `.config load <名称>` | 加载配置 |

### 脚本示例

在 `~/.zen/liquidres/scripts/` 创建 `HelloWorld.js`：

```javascript
var mod = createModule("HelloWorld", Category.MISC, {
  onKey: function(e) {
    if (e.isPressed() && e.getKeyCode() == 295) {
      printChat("§aHello, Amadeus!");
    }
  }
});
mod.setKey(295); // F6
保存后执行 .script reload HelloWorld，按 F6 即可输出消息。

文档
API 参考 – 完整脚本文档

事件列表、预绑定变量、工具类、示例代码、常见陷阱

从源码构建
bash
git clone https://github.com/AmadeusClient/AmadeusClient.git
cd AmadeusClient
./gradlew build
构建产物位于 build/libs/

贡献
Fork 本仓库

创建特性分支 (git checkout -b feature/AmazingFeature)

提交改动 (git commit -m 'Add some AmazingFeature')

推送分支 (git push origin feature/AmazingFeature)

打开 Pull Request

社区
QQ 群：617996394

Issues：https://github.com/AmadeusClient/AmadeusClient/issues

Discussions：https://github.com/AmadeusClient/AmadeusClient/discussions

许可证
MIT License © Amadeus Client

持续更新 · 所有功能以实际版本为准

text
将你写的md最外层用{}包裹起来
我们需要将上面提供的 README.md 内容用大括号包裹起来。也就是说，整个 Markdown 文本需要被一个外层的 {} 包围。注意，Markdown 文本本身包含反引号、井号等，但最外层加上大括号后，整个内容就变成了一个代码块或者文本块。由于是 Markdown 文件，通常不会这样用，但用户要求，我们就照做。

我们需要把上面最后一次生成的 README.md 的完整内容（从第一行到末尾）用 { 和 } 包起来。注意要保留所有换行和格式。

我将在回答中直接输出包裹后的内容。确保大括号在开头和结尾，独占一行或紧跟内容均可，但为了让格式清晰，我选择在开头单独一行 {，然后接内容，最后单独一行 }。

同时要确保内容没有丢失任何部分。

text
# Amadeus Client

高性能 Minecraft 客户端 · 模块化架构 · 内置 GraalJS 脚本引擎

---

## 简介

Amadeus 是一款为 **PVP** 与 **实用功能** 而生的 Minecraft 客户端。采用模块化设计，内置 **GraalJS** 脚本引擎，支持 JavaScript 扩展，轻量高效，高度可定制。

- **官网**：https://amadeusclient.github.io  
- **API 文档**：https://amadeusclient.github.io/api.html  
- **下载**：https://github.com/AmadeusClient/AmadeusClient/releases

---

## 核心特性

- **极致性能** – ASM 字节码优化，极低资源占用
- **模块化设计** – 60+ 独立模块，六大分类，按需开关
- **脚本扩展** – GraalJS 引擎，热重载，无需重启
- **动态 HUD** – 完全拖拽式布局，自由定制
- **丰富设置** – 每个模块独立设置面板
- **安全稳定** – 严格沙箱，上下文隔离

---

## 安装

### 环境要求
- Minecraft 1.20.4
- Java 17+
- Forge 47.x+ 或 Fabric 0.15+

### 步骤
1. 从 [Releases](https://github.com/AmadeusClient/AmadeusClient/releases) 下载最新 `.jar`
2. 放入 `.minecraft/mods/` 目录
3. 启动游戏，按 `RSHIFT` 或 `F6` 打开 ClickGUI

---

## 快速开始

| 操作 | 按键 |
|------|------|
| 打开 ClickGUI | `RSHIFT` / `F6` |
| HUD 编辑模式 | `Ctrl + H` |
| 模块绑键 | ClickGUI 中点击绑定区域 |

### 常用命令

| 命令 | 说明 |
|------|------|
| `.clickgui` | 打开 ClickGUI |
| `.hud` | 打开 HUD 编辑器 |
| `.script load <文件名>` | 加载脚本 |
| `.script reload <脚本名>` | 热重载脚本 |
| `.script reloadall` | 重载所有脚本 |
| `.script list` | 列出已加载脚本 |
| `.vclip <距离>` | 垂直传送 |
| `.hclip <距离>` | 水平传送 |
| `.friend add/remove <玩家>` | 管理好友 |
| `.panic` | 紧急禁用所有模块 |
| `.config save <名称>` | 保存配置 |
| `.config load <名称>` | 加载配置 |

### 脚本示例

在 `~/.zen/liquidres/scripts/` 创建 `HelloWorld.js`：

```javascript
var mod = createModule("HelloWorld", Category.MISC, {
  onKey: function(e) {
    if (e.isPressed() && e.getKeyCode() == 295) {
      printChat("§aHello, Amadeus!");
    }
  }
});
mod.setKey(295); // F6
保存后执行 .script reload HelloWorld，按 F6 即可输出消息。

文档
API 参考 – 完整脚本文档

事件列表、预绑定变量、工具类、示例代码、常见陷阱

从源码构建
bash
git clone https://github.com/AmadeusClient/AmadeusClient.git
cd AmadeusClient
./gradlew build
构建产物位于 build/libs/

贡献
Fork 本仓库

创建特性分支 (git checkout -b feature/AmazingFeature)

提交改动 (git commit -m 'Add some AmazingFeature')

推送分支 (git push origin feature/AmazingFeature)

打开 Pull Request

社区
QQ 群：617996394

Issues：https://github.com/AmadeusClient/AmadeusClient/issues

Discussions：https://github.com/AmadeusClient/AmadeusClient/discussions

许可证
MIT License © Amadeus Client

持续更新 · 所有功能以实际版本为准

text
