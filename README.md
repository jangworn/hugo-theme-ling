# hugo-theme-ling
基于[hyde](https://github.com/spf13/hyde) 修改的主题，增加了搜索、翻页等功能

## 截图
![theme](images/theme.png)

## 安装
```
$ cd your_site_repo/
$ mkdir themes
$ cd themes
$ git clone https://github.com/jangworn/hugo-theme-ling ling

```
## 启动
修改config.toml   
theme = "ling"
```
$ hugo server --buildDrafts
```

## 我的config.toml
```
baseURL = "http://example.org/"
languageCode = "en-us"
title = "后会有期"
theme="ling"
paginate = 10
paginatePath = "page"
hasCJKLanguage="true"
titleCaseStyle = "Go"
[permalinks]
  post = "/:year/:month/:day/:title/"
[params]
  themeColor = "theme-cyan"
  description = "青山不改，绿水长流"
[Menus]
  main = [
      {Name = "Github", URL = "https://github.com/jangworn/"}
  ]
[markup]
  [markup.highlight]
    codeFences = true
    guessSyntax = true
    hl_Lines = ""
    lineNoStart = 1
    lineNos = true
    lineNumbersInTable = false
    noClasses = true
    style = "monokai"
    tabWidth = 4
[outputs]
  home = ["HTML", "RSS", "JSON"]

```