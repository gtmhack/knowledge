## 文件编码

请调整您的文件编码为 UTF-8 without BOM


## 换行符

请使用UNIX风格的换行符，即 "\n"


## 缩进

代码缩进使用的是4个空格，不使用制表符(tab)


## 行尾空白

行尾不要保留空格或tab

-----------

如果你使用`Sublime Text`可在配置文件中添加以下项，编辑器会自动完成以上要求

```JSON
{
    "default_line_ending": "unix",
    "tab_size": 4,
    "translate_tabs_to_spaces": true,
    "trim_trailing_white_space_on_save": true,
    "ensure_newline_at_eof_on_save": true
}

````
