## 学习记录
#### 🤔 To Do List
- [ ] 暂无

#### 💡 当前状态
- 可用，概率 renew 🍑

#### 🍳 烹饪方法：1.1 
- Settings > Secrets > Actions 添加以下变量

|YOU SECRET NAME|YOU SECRET VALUE|
|-----|-----|
|`USER_ID`|你的 id|
|`PASS_WD`|你的密码|
|`BARK_KEY`|(可选) https://api.day.app/BARK_KEY/|
|`TG_BOT_TOKEN`|(可选) `xxxxxx:xxxxxxxxxxxxx`|
|`TG_USER_ID`|(可选) 给 bot `@userinfobot` 发送 `/start`|

#### 🍳 烹饪方法：1.2 
- Actions > Workflows [*-Extend] > Run workflow
- <img src=./step.png width=50% />

#### 📖 触发说明：手动 + schedule
```
name: '*-Extend'

on:
  #push:
  schedule:
    # run everyday at UTC 04:30 (CN time UTC+8)
     - cron: '30 4 * * *'
  # Allows you to run this workflow manually from the Actions tab
  workflow_dispatch:
```

#### ❓ 运行结果
```
*** 💣 Possibly blocked by google! ***
Your computer or network may be sending automated queries. To protect our users, we can't process your request right now. For more details visit our help page.
```
or
```
 🎉 Your VPS has been renewed until ****
```
<img src=./result.png width=50% />

#### 📚 资料参考
- https://www.python.org/
- https://www.selenium.dev/
- https://www.youtube.com/watch?v=As-_hfZUyIs
- https://github.com/actions/virtual-environments/blob/main/images/macos/macos-12-Readme.md
- https://github.com/mherrmann/selenium-python-helium/blob/master/helium/__init__.py
