# JavaScript 编辑器选择

## 主流开发编辑器

- [VSCode](https://code.visualstudio.com/)
- [Sublime](http://www.sublimetext.com/)
- 其它

```nginx
# 个人比较喜欢这 2 款轻便型的开发编辑器

# 如有其它喜好的开发编辑器,请自行下载 ...
```





### VSCode

#### 插件库

```nginx
% VSCode 必备 %
# vscode-icons (vscode 目录图标)
# Settings Sync (上传|下载 VSCode 配置文件)
# Chinese Language Pack for Visual Studio Code (编辑器汉化包,凭个人喜好)

% 前端开发必备 %
# HTML CSS Support
# HTML Snippets
# Auto Close Tag (自动完成补全标签)
# Auto Rename Tag （自动完成标签重命名）
# Code Runder (快速运行代码块,支持多语言)
# IntelliSence for CSS class names in HTML
# JavaScript(ES6) code snippets
# JavaScript and TypeScript Nightly
# Path Intellisence
# Visual Studio IntelliCode
# Trailing Spaces (去除多余的前后空格)
# Debugger for Chrome (谷歌调试器)
# open in browser (打开默认浏览器)

% 项目版本管理必备 %
# Git Blame
# Git History
# GitLens - Git supercharged
# npm Intellisence

% Vue 技术栈必备 %
# Vetur
# Vue 3 Snippets
# Vue Language Features(Volar)

% React 技术栈必备 %

% 微信小程序开发必备 %
# wechat-snipets

% TypeScript 技术栈必备 %
# TypeScript Hero

% ThreeJs 3D 开发必备 %
# ThreeJs Snippets

% Markdown 文档编写必备 % 
# Markdown Preview Enhanced

% 代码格式化必备 % 
# Prettier - Code formmatter

% 辅助必备 %
# filesize (文件大小)
# Image preview (图片预览)
# Svg Viewer (SVG 文件预览)
```



#### 插件配置

settings.json

```json
{
  /* vscode 编辑器配置 */
  "editor.fontSize": 12,
  "editor.tabSize": 2,
  "editor.wordWrap": "on",
  "editor.suggestSelection": "first",
  /* 保存时自动格式化 */
  "editor.formatOnSave": true,
  /* prettier 代码格式检查配置 */
  /* 单引号 */
  "prettier.singleQuote": true,
  /* 尾部添加分号 */
  "prettier.semi": true,
  /** 缩进长度 */
  "prettier.tabWidth": 2,
  /* 使用 tab 缩进 */
  "prettier.useTabs": false,
  /* 空格替代 tab */
  "prettier.bracketSpacing": true,
  /* 箭头参数可省略括号 */
  "prettier.arrowParens": "avoid",
  /* jsx 标签对齐 */
  "prettier.jsxBracketSameLine": false,
  /** 是否缩进 script, style */
  "prettier.vueIndentScriptAndStyle": false,
  /** prettier 格式化配置 */
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[vue]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  /* vscode-icons 配置*/
  "workbench.iconTheme": "vscode-icons",
  /* 其它配置 */
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",

  /** git-bash 配置 */
  "terminal.integrated.profiles.windows": {
    "PowerShell": {
      "source": "PowerShell",
      "icon": "terminal-powershell"
    },
    "Command Prompt": {
      "path": [
        "${env:windir}\\Sysnative\\cmd.exe",
        "${env:windir}\\System32\\cmd.exe"
      ],
      "args": [],
      "icon": "terminal-cmd"
    },
    "Git Bash": {
      "source": "Git Bash"
    },
    "bash": {
      "path": "D:\\Git\\bin\\bash.exe",
      "args": []
    }
  },
  "terminal.integrated.defaultProfile.windows": "bash"
}

```





### Sublime

#### 插件库

```nginx
% Sublime 必备 %
# Package Control
# A File Icon
# zzz A File Icon zzz
# ConvertToUTF8
# SublimeCodeIntel
# SublimeLinter
# SublimeTmpl

% 前端开发必备 %
# HTML5
# CSS3
# SCSS
# Emmet
# Babel
# Import Const
# AutoFileName
# All Autocomplete
# View I Browser

% 服务端开发必备 %
# Nodejs

% Vue 技术栈必备 %
# Vue Syntax Higtlight

% 代码格式化必备 % 
# JsPrettier

% 辅助必备 %
# DocBlockr (文档说明)

```



#### 插件配置

Preferences => Key bindings =>  Default.sublime.keymap

```json
[
    /** 命令行面板 */
	{ "keys": ["alt+`"], "command": "toggle_terminus_panel" },
    /** 格式化 JS 代码 */
	{ "keys": ["shift+alt+f"], "command": "js_prettier" }
]
```

