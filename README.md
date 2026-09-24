<div align="center">

<img src="icon.png" alt="屿宸网络科技工作室" width="220" />

<br />

<sub>

**CURSOR 汉化组** · CURSOR CHINESE TRANSLATION GROUP

</sub>

</div>

---

# Visual Studio Code 简体中文语言包

本插件面向 **Visual Studio Code** 与 **Cursor** 编辑器，基于官方简体中文语言包基线，整合社区翻译与持续维护更新，为菜单、设置、命令面板、通知、调试面板及内置扩展提供完整的中文界面体验。

✨ **当前版本 1.0.0**

VS Code 1.90+ · Language Pack · 约 **2.8 万条** 界面词条 + 社区补齐

---

## 项目亮点

- 🎯 **全量汉化** — 覆盖 VS Code 核心界面与 90+ 内置扩展模块，包括菜单、设置、命令、通知、调试与终端等
- 🔒 **零侵入安装** — 纯语言包扩展，不修改编辑器安装目录，无需管理员权限
- 🌏 **官方基线** — 基于 [microsoft/vscode-loc](https://github.com/microsoft/vscode-loc) 简体中文翻译，增量维护避免重复劳动
- ⚡ **安装即用** — 安装后执行「配置显示语言」选择「中文(简体)」，重启编辑器即可生效
- 📊 **持续更新** — 跟踪 VS Code 新版本词条变化，及时同步翻译
- 📜 **持续维护** — 由 **屿宸网络科技工作室 / CURSOR 汉化组** 维护

---

<div align="center">

![version](https://img.shields.io/badge/version-1.0.0-1a73e8?style=flat-square)
![type](https://img.shields.io/badge/type-Language%20Pack-34a853?style=flat-square)
![license](https://img.shields.io/badge/license-MIT-9aa0a6?style=flat-square)
![locale](https://img.shields.io/badge/locale-zh--CN-e8710a?style=flat-square)
![vscode](https://img.shields.io/badge/VS%20Code-1.90%2B-0078d4?style=flat-square)

</div>

---

## 安装方式

### 方式一：从 VSIX 安装（推荐）

1. 下载或自行打包 `vscode-chinese-1.0.0.vsix`
2. 打开 VS Code / Cursor，按 `Ctrl+Shift+P` 打开命令面板
3. 输入并选择 **Extensions: Install from VSIX...**（从 VSIX 安装扩展）
4. 选择下载的 `.vsix` 文件完成安装

### 方式二：从源码打包

```bash
npm install -g @vscode/vsce
vsce package
```

### 方式三：从 GitHub 克隆

```bash
git clone https://github.com/Ms-liyc/VScode-Chinese.git
cd VScode-Chinese
vsce package
```

---

## 切换为中文界面

1. 按 `Ctrl+Shift+P` 打开命令面板
2. 输入 **Configure Display Language**（配置显示语言）
3. 选择 **中文(简体)** / `zh-cn`
4. 按提示 **重启** 编辑器

也可在 `locale.json` 中手动设置：

```json
{
  "locale": "zh-cn"
}
```

文件位置：

- **Windows**: `%APPDATA%\Code\User\locale.json`
- **macOS**: `~/Library/Application Support/Code/User/locale.json`
- **Linux**: `~/.config/Code/User/locale.json`

---

## 说明

本插件**仅替换界面显示文本**，不修改编辑器核心程序与任何业务逻辑。建议通过「从 VSIX 安装扩展」或扩展市场安装。

> ⚠️ **注意**
>
> - 若已安装微软官方「Chinese (Simplified) Language Pack」，建议**禁用或卸载**以避免语言包冲突
> - 修改显示语言后需**重启编辑器**才能完全生效
> - Cursor 用户同样适用，安装后按上述步骤切换语言即可

---

## 目录结构

```
VScode-Chinese/
├── icon.png              # 扩展图标
├── package.json          # 扩展清单
├── translations/         # 翻译资源
│   ├── main.i18n.json    # VS Code 核心界面
│   └── extensions/       # 内置扩展翻译
├── assets/               # README 资源
├── LICENSE.md
└── README.md
```

---

## 致谢

- 翻译基线来源：[microsoft/vscode-loc](https://github.com/microsoft/vscode-loc)
- 开发者：[屿宸网络科技工作室](https://github.com/Ms-liyc/VScode-Chinese)

---

## 许可证

本项目采用 [MIT License](./LICENSE.md) 开源协议。
