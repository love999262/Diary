# VScode可以说是目前最强大的文本编译器,配合一些插件,完全可以与IDE媲美,并且非常的流畅,可以说是地球上第二强大的编辑器也不为过.

- 首先进入官网[VSCode](https://code.visualstudio.com/),下载对应系统的VSCode.

- 然后安装插件`Ctrl/Cmd+P`之后`ext install`

- 下面给出一些常用插件:

```
Auto Close Tag 自动闭合HTML标签

Auto Rename Tag 修改HTML标签时，自动修改匹配的标签

Bookmarks 添加行书签

Can I Use HTML5、CSS3、SVG的浏览器兼容性检查

Code Runner 运行选中代码段（支持大量语言，包括Node）

CodeBing 在VSCode中弹出浏览器并搜索，可编辑搜索引擎

Color Highlight 颜色值在代码中高亮显示

Color Picker 拾色器

Document This 注释文档生成

EditorConfig for VS Code EditorConfig 插件

Emoji 在代码中输入emoji

ESLint ESLint插件，高亮提示

File Peek 根据路径字符串，快速定位到文件

Font-awesome codes for html FontAwesome提示代码段

ftp-sync 同步文件到ftp

Git Blame 在状态栏显示当前行的Git信息

Git History(git log) 查看git log

GitLens 显示文件最近的commit和作者，显示当前行commit信息

Guides 高亮缩进基准线

Gulp Snippets Gulp代码段

HTML CSS Class Completion CSS class提示

HTML CSS Support css提示（支持vue）

HTMLHint HTML格式提示

Indenticator 缩进高亮

JavaScript (ES6) code snippets ES6语法代码段

language-stylus Stylus语法高亮和提示

Lodash Lodash代码段

markdownlint Markdown格式提示

MochaSnippets Mocha代码段

Node modules resolve 快速导航到Node模块

npm 运行npm命令

npm Intellisense 导入模块时，提示已安装模块名称

Output Colorizer 彩色输出信息

Partial Diff 对比两段代码或文件

Path Autocomplete 路径完成提示

Path Intellisense 另一个路径完成提示

Prettify JSON 格式化JSON

Project Manager 快速切换项目

REST Client 发送REST风格的HTTP请求

Settings Sync VSCode设置同步到Gist

String Manipulation 字符串转换处理（驼峰、大写开头、下划线等等）

Test Spec Generator 测试用例生成（支持chai、should、jasmine）

TODO Parser Todo管理

Version Lens package.json文件显示模块当前版本和最新版本

vetur 目前比较好的Vue语法高亮

View Node Package 快速打开选中模块的主页和代码仓库

vscode-icons 文件图标，方便定位文件

VSCode Great Icons 文件图标拓展

VueHelper Vue2代码段（包括Vue2 api、vue-router2、vuex2）

View InBrowser 在浏览器中打开
```


快捷键:↑↓←→

进入对应函数:

```
Ctrl + 鼠标左键
```
进入后回到上次的地方:
```
Ctrl + Alt + ←/→
```
markdown预览:
```
Ctrl+Shift+V
```

文件查找

在当前文件查找文本

在当前文件替换文本

在当前项目查找文本

删除一行

剪切 

复制/粘贴
```
// 将键绑定放入此文件中以覆盖默认值
[
    {
        "key": "alt+d",
        "command": "editor.action.addSelectionToNextFindMatch",
        "when": "editorFocus"
    },
    {
        "key": "ctrl+d",
        "command": "-editor.action.addSelectionToNextFindMatch",
        "when": "editorFocus"
    },
    {
        "key": "ctrl+r",
        "command": "editor.action.startFindReplaceAction"
    },
    {
        "key": "ctrl+h",
        "command": "-editor.action.startFindReplaceAction"
    },
    {
        "key": "ctrl+d",
        "command": "editor.action.deleteLines",
        "when": "textInputFocus && !editorReadonly"
    },
    {
        "key": "ctrl+shift+k",
        "command": "-editor.action.deleteLines",
        "when": "textInputFocus && !editorReadonly"
    },
    {
        "key": "ctrl+shift+r",
        "command": "workbench.action.replaceInFiles"
    },
    {
        "key": "ctrl+shift+h",
        "command": "-workbench.action.replaceInFiles"
    },
    {
        "key": "ctrl+alt+c",
        "command": "editor.action.formatSelection",
        "when": "editorHasSelection && editorTextFocus && !editorReadonly"
    },
    {
        "key": "ctrl+k ctrl+f",
        "command": "-editor.action.formatSelection",
        "when": "editorHasSelection && editorTextFocus && !editorReadonly"
    },
    {
        "key": "ctrl+shift+c",
        "command": "workbench.action.terminal.new"
    },
    {
        "key": "ctrl+shift+oem_3",
        "command": "-workbench.action.terminal.new"
    }
]

// 将按键绑定配置放入此文件中即可覆盖默认值
+[
+    {
+        "key": "alt+d",
+        "command": "editor.action.addSelectionToNextFindMatch",
+        "when": "editorFocus"
+    },
+    {
+        "key": "cmd+d",
+        "command": "-editor.action.addSelectionToNextFindMatch",
+        "when": "editorFocus"
+    },
+    {
+        "key": "cmd+r",
+        "command": "editor.action.startFindReplaceAction"
+    },
+    {
+        "key": "alt+cmd+f",
+        "command": "-editor.action.startFindReplaceAction"
+    },
+    {
+        "key": "alt+left",
+        "command": "workbench.action.navigateBack"
+    },
+    {
+        "key": "ctrl+-",
+        "command": "-workbench.action.navigateBack"
+    },
+    {
+        "key": "alt+right",
+        "command": "workbench.action.navigateForward"
+    },
+    {
+        "key": "ctrl+shift+-",
+        "command": "-workbench.action.navigateForward"
+    },
+    {
+        "key": "cmd+d",
+        "command": "editor.action.deleteLines",
+        "when": "textInputFocus && !editorReadonly"
+    },
+    {
+        "key": "shift+cmd+k",
+        "command": "-editor.action.deleteLines",
+        "when": "textInputFocus && !editorReadonly"
+    },
+    {
+        "key": "shift+cmd+r",
+        "command": "workbench.action.replaceInFiles"
+    },
+    {
+        "key": "shift+cmd+h",
+        "command": "-workbench.action.replaceInFiles"
+    }
+]

```
