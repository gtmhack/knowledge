## fix bug一定要找到root cause

[Linux 2.6.39-rc3的一个插曲 from CoolShell](http://coolshell.cn/articles/4576.html)


## 不要注释无用代码

一是增加了搜索时无用的结果，二是给维护增加了很多困难

保存旧代码是版本管理工具的工作


## YAGNI 原则

[You aren't gonna need it](http://en.wikipedia.org/wiki/You_aren't_gonna_need_it)


## Tell, Don't Ask
bad:
```
<% if current_user.admin? %>
  <%= current_user.admin_welcome_message %>
<% else %>
  <%= current_user.user_welcome_message %>
<% end %>
```
good:
```
<%= current_user.welcome_message %>
```
