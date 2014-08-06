# xtpl emmet

借助强大的 Emmet 插件，提供 [KISSY xTemplate](http://kissyteam.github.io/xtpl/) 中常用代码片段，从而提高开发效率。

## 使用方法

基于 Emmet 插件，以 Sublime text 为例：

1. 确保已经安装了 Emmet 插件，并且可以正常使用
2. 打开菜单 `Preferences`→`Package Settings`→`Emmet`→`Settings-User`
3. 复制 `Emmet.sublime-settings` 文件中的所有内容，粘贴到上面打开的 `Settings-User` 中（如果之前存在内容，请按照格式合并即可）
4. Enjoy It！

## 支持文件类型

1. HTML 类型文件
2. xtpl 后缀文件（需要安装[xtpl-sublime](https://github.com/kissyteam/xtpl-sublime)）
3. 其他使用 `Set Syntax: HTML` 或  `Set Syntax: XTpl` 命令的文件 


## 支持短代码列表

- `x`：快速生成 `{{}}` 方括号并聚焦其中，再敲击 Tab 跳出
- `xif`：生成 `{{#if( condition )}}//code...{{/if}}` 普通 if 语句
- `xife`：生成 `{{#if( condition )}}//code...{{else}}//code...{{/if}}` 带有 else 的 if 语句
- `xif+`：生成 `{{#if( condition )}}//code...{{elseif( condition )}}//code...{{else}}//code...{{/if}}` 更复杂的 if 语句
- `xeach`：生成 `{{#each([1,2,4])}}{{this}}{{/each}}` 普通的 each 循环语句
- `xeachi`：生成 `{{#each([1,2,4])}}{{xindex}}{{this}}{{/each}}` 带有 xindex 的循环语句
- `xeachr`：生成 `{{#each(range(1,2))}}{{this}}{{/each}}` 循环一个范围内的循环语句
- `x%`：生成 `{{%  %}}` 用于原样输出模版（单行）
- `x%+`：生成 `{{%  %}}` 用于原样输出模版（多行）
- `xcm`：生成 `{{! content }}` 模版评论
- `xcm[content=注释内容]`：生成 `{{! 注释内容 }}`
- `xs`：生成 `{{set(e)}}` 设置变量
- `xs[e=y=3,x=4]`：生成 `{{set(y=3,x=4)}}`，注意 `e=` 后面表达式不要添加任何空格
- `xs[e=z=4]`：生成 `{{set(z=4)}}`
- `xm`：生成 `{{#macro(params)}}param is ...{{/macro}}` 配置宏
- `xmd`：生成 `{{macro(params)}}` 调用某配置的宏
- `xi`：生成 `{{include ("include files")}}` 引入文件
- `xe`：生成 `{{extend ("extend files")}}` 继承文件
- `xb`：生成 `{{#block ("block name")}}code...{{/block}}` 快
- `xw`：生成 `{{#with({x:2})}}{{x}}{{/with}}`


## 问题反馈

还缺什么命令，或者某些段代码的不够方便等等，欢迎到 Issues 里面讨论，或者 PR。

MIT



