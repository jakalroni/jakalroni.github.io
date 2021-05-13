---
title: 블로그에 소스코드 첨부
tags: etc
key: page-202105140248
summary : 소스코드 첨부방법
---

## GitHub 블로그에 Source Code 첨부해보기!
[https://syki66.github.io/blog/2020/04/16/TeXt-theme-config.html](https://syki66.github.io/blog/2020/04/16/TeXt-theme-config.html)
<br>
위 블로그를 참조해보자.
</br>

```Ruby
## => Site Settings
##############################
text_skin: forest # 사이트 테마 "default" (default), "dark", "forest", "ocean", "chocolate", "orange"
highlight_theme: tomorrow-night-eighties # 코드블럭 테마 "default" (default), "tomorrow", "tomorrow-night", "tomorrow-night-eighties", "tomorrow-night-blue", "tomorrow-night-bright"
url     : https://jakalroni.github.io # baseurl이 존재하면 적기 the base hostname & protocol for your site e.g. https://www.someone.com
baseurl : # does not include hostname
title   : ChamCham2 #사이트 이름
description: > # 사이트 상세정보 this means to ignore newlines until "Language & timezone"
  나의 개발 기록 블로그


## => Language and Timezone
##############################
lang: ko-KR # the language of your site, default as "en"
timezone: Asia/Seoul # see https://en.wikipedia.org/wiki/List_of_tz_database_time_zones for the available values


## => Author and Social 저자 정보를 알맞게 쓰면됨
##############################
author:
  type      : # "person" (default), "organization"
  name      : jakalroni
  url       : https://jakalroni.github.io
  avatar    : # path or url of avatar image (square)
  bio       : Dankook.UNIV SoftWare Department 18th
  email     : jakalroni@naver.com
  facebook  : # "user_name" the last part of your profile url, e.g. https://www.facebook.com/user_name
  twitter   : # "user_name" the last part of your profile url, e.g. https://twitter.com/user_name
  weibo     : # "user_id"   the last part of your profile url, e.g. https://www.weibo.com/user_id/profile?...
  googleplus: # "user_id"   the last part of your profile url, e.g. https://plus.google.com/u/0/user_id
  telegram  : # "user_name" the last part of your profile url, e.g. https://t.me/user_name
  medium    : # "user_name" the last part of your profile url, e.g. https://medium.com/user_name
  zhihu     : # "user_name" the last part of your profile url, e.g. https://www.zhihu.com/people/user_name
  douban    : # "user_name" the last part of your profile url, e.g. https://www.douban.com/people/user_name
  linkedin  : # "user_name" the last part of your profile url, e.g. https://www.linkedin.com/in/user_name
  github    : jakalroni # "user_name" the last part of your profile url, e.g. https://github.com/user_name
  npm       : # "user_name" the last part of your profile url, e.g. https://www.npmjs.com/~user_name


## => GitHub Repository (if the site is hosted by GitHub) 블로그의 깃허브 레포지토리 적기
##############################
repository: jakalroni/jakalroni.github.io #user_name/repo_name
repository_tree: master


## => Paths
##############################
paths:
  root    : # title link url, "/" (default)
  home    : # home layout url, "/" (default)
  archive : # "/archive.html" (default)
  rss     : # "/feed.xml" (default)


## => Post
##############################
## excerpt 자동으로 본문 발췌시 구분점을 어떤것으로 할지 정하기
excerpt_separator: <!--more-->

## license
license: # "CC-BY-4.0", "CC-BY-SA-4.0", "CC-BY-NC-4.0" (default), "CC-BY-ND-4.0"

## TOC 사이드 네비게이션에 넣을 태그 선택
toc:
  selectors: # "h1,h2,h3" (default)


## => Markdown Enhancements
##############################
## Mathjax
mathjax: # false (default), true
mathjax_autoNumber: # false (default), true

## Mermaid
mermaid: # false (default), true

## Chart
chart: # false (default), true


## => Paginate 한 페이지에 보여줄 post 개수
##############################
paginate: 8
paginate_path: /page:num # don't change this unless for special need


## => Sources
##############################
sources: # bootcdn (default), unpkg


## => Sharing
##############################
sharing:
  provider: false # false (default), "addtoany", "addthis", "custom"

  ## AddThis
  addthis:
    id: # AddThis pubid, e.g. ra-5xxxxxxxxxxx


## => Comments 댓글 공급자 선택하기
##############################
comments:
  provider: false # false (default), "disqus", "gitalk", "valine", "custom"

  ## Disqus
  disqus:
    shortname: # the Disqus shortname for the site

  ## Gitalk
  # please refer to https://github.com/gitalk/gitalk for more info.
  gitalk:
    clientID    : # GitHub Application Client ID
    clientSecret: # GitHub Application Client Secret
    repository  : # GitHub repo
    owner       : # GitHub repo owner
    admin: # GitHub repo owner and collaborators, only these guys can initialize GitHub issues, IT IS A LIST.
      # - your GitHub Id

  ## Valine
  # please refer to https://valine.js.org/en/ for more info.
  valine:
    app_id      : # LeanCloud App id
    app_key     : # LeanCloud App key
    placeholder : # Prompt information
    visitor     : # false (default)
    meta        : # "[nick, mail, link]" (default) nickname, E-mail, Personal-site


## => Pageview
##############################
pageview:
  provider: false # false (default), "leancloud", "custom"

  ## Leancloud
  leancloud:
    app_id    : # LeanCloud App id
    app_key   : # LeanCloud App key
    app_class : # LeanCloud App class


## => Search
##############################
search:
  provider: default # "default" (default), false, "google", "custom"

  ## Google Custom Search Engine
  google:
    custom_search_engine_id: # Google Custom Search Engine ID


## => Analytics
##############################
analytics:
  provider: false # false (default), "google", "custom"

  ## Google Analytics
  google:
    tracking_id : # Google Analytics id for the site
    anonymize_ip: false # Anonymize IP tracking for Analytics


## => Build
##############################
markdown    : kramdown
highlighter : rouge
permalink   : date

exclude:
  - CHANGELOG.md
  - HOW_TO_RELEASE.md
  - Gemfile
  - Gemfile.lock
  - LICENSE
  - README-*.md
  - README.md
  - gulpfile.js
  - jekyll-text-theme.gemspec
  - package-lock.json
  - package.json
  - /docs
  - /node_modules
  - /screenshots
  - /test
  - /vendor

# 레이아웃 기본값 설정 (자신의 기호에 맞게 넣으면됨)
defaults:
  - scope:
      path: ""
      type: posts
    values:
      layout: article # post의 레이아웃, article로 설정해야됨
      title: Page - Single
      sharing: true # 공유 표시
      license: true # 라이센스 표시
      aside:
        toc: true # 사이드 메뉴 활성화
      show_edit_on_github: true
      show_subscribe: true # feed.xml 하단부에 띄울건지
      pageview: true
      key: anything # 반드시 이 구문을 넣어야 disqus 댓글이 각 post 마다 실행됨
      mode: immersive # 백그라운드 이미지 위에 헤더와 타이틀 올리기
      header:
        theme: dark # dark는 헤더의 배경을 어둡게 하고 글씨를 밝게함. light는 반대
      article_header:
        type: overlay # 포스트 내부에서 헤더 오버레이 적용여부
        theme: dark
        background_image: # 포스트 헤더 배경이미지 경로 및 그라데이션 설정
          src: https://user-images.githubusercontent.com/59393359/74720914-e4b7e980-5279-11ea-9532-c262caf64f00.jpg
          gradient: 'linear-gradient(rgba(0, 0, 0, .3), rgba(0, 0, 0, .0))'



## => Plugins
##############################
plugins:
  - jekyll-feed
  - jekyll-paginate
  - jekyll-sitemap
  - jemoji
```