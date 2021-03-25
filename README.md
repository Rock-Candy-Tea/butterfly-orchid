# butterfly_orchid1.0


## 包含6款插件:

#### Hexo Github Canlendar
link: https://zfe.space/post/hexo-githubcalendar.html
![image](https://user-images.githubusercontent.com/19563906/112476126-8b8b8500-8dac-11eb-960d-f6b7f8c24594.png)
---
#### Hexo Magnet
link: https://zfe.space/post/hexo-magnet.html
![image](https://user-images.githubusercontent.com/19563906/112476197-9e9e5500-8dac-11eb-9929-43b75ee33b6d.png)
---
#### Hexo Swiper
link: https://zfe.space/post/hexo-swiper.html
![image](https://user-images.githubusercontent.com/19563906/112476240-a958ea00-8dac-11eb-9695-0a7f9165d45e.png)
---
#### Butterfly Article Double Row
link: https://zfe.space/post/hexo-butterfly-article-double-row.html
![image](https://user-images.githubusercontent.com/19563906/112476289-b544ac00-8dac-11eb-898a-0cf380bb6d9f.png)
---
#### Hexo History Calendar
link: https://zfe.space/post/hexo-history-calendar.html
![image](https://user-images.githubusercontent.com/19563906/112476360-c68db880-8dac-11eb-89df-8f5034078409.png)
---
#### Hexo Electric Clock
link: https://zfe.space/post/hexo-electric-clock.html
![image](https://user-images.githubusercontent.com/19563906/112476395-cf7e8a00-8dac-11eb-96df-481f3e52fed2.png)
---

## 安装命令:

```powershell
npm i hexo-githubcalendar hexo-magnet hexo-swiper-bar hexo-butterfly-article-double-row hexo-history-calendar hexo-electric-clock --save
```

## 将以下内容放入博客根目录的config中即可。

```yaml
# Ice Kano Plus_in
# Hexo Github Canlendar
# Volantis
# Matery
# butterfly
githubcalendar:
  enable: true
  priority: 3
  enable_page: /
  user: zfour
  layout:
    type: id
    name: recent-posts
    index: 0
  githubcalendar_html: '<div class="recent-post-item" style="width:100%;height:auto;padding:10px;"><div id="github_loading" style="height:100%;display: flex;align-items: center;justify-content: center;"><svg style="height:50px" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"  viewBox="0 0 50 50" style="enable-background:new 0 0 50 50" xml:space="preserve"><path fill="#d0d0d0" d="M25.251,6.461c-10.318,0-18.683,8.365-18.683,18.683h4.068c0-8.071,6.543-14.615,14.615-14.615V6.461z" transform="rotate(275.098 25 25)"><animateTransform attributeType="xml" attributeName="transform" type="rotate" from="0 25 25" to="360 25 25" dur="0.6s" repeatCount="indefinite"></animateTransform></path></svg></div><div id="github_container"></div></div>'
  pc_minheight: 248px
  mobile_minheight: 0px
  color: "['#ebedf0', '#fdcdec', '#fc9bd9', '#fa6ac5', '#f838b2', '#f5089f', '#c4067e', '#92055e', '#540336', '#48022f', '#30021f']"
  api: https://python-github-calendar-api.vercel.app/api
  # api: https://python-gitee-calendar-api.vercel.app/api
  calendar_js: https://cdn.jsdelivr.net/gh/Zfour/hexo-github-calendar@1.21/hexo_githubcalendar.js
  plus_style: ""

magnet:
  enable: true
  priority: 1
  enable_page: all
  type: categories
  devide: 2
  display:
    - name: 教程
      display_name: 小冰の魔改教程
      icon: 📚
    - name: 游戏评测
      display_name: 小冰の游戏评测
      icon: 🎮
    - name: 生活趣闻
      display_name: 小冰の生活趣闻
      icon: 🐱‍👓
    - name: vue
      display_name: 小冰の编程学习
      icon: 👩‍💻
    - name: 学习
      display_name: 小冰の读书笔记
      icon: 📒
    - name: 随想
      display_name: 小冰の胡思乱想
      icon: 💡
  color_setting:
    text_color: black
    text_hover_color: white
    background_color: '#f2f2f2'
    background_hover_color: '#b30070'
  layout:
    type: id
    name: recent-posts
    index: 0
  temple_html: '<div class="recent-post-item" style="width:100%;height: auto"><div id="catalog_magnet">${temple_html_item}</div></div>'
  plus_style: ""


swiper:
  enable: true
  priority: 2
  enable_page: /
  layout:
    type: id
    name: recent-posts
    index: 0
  temple_html: '<div class="recent-post-item" style="height: auto;width: 100%"><div class="blog-slider swiper-container-fade swiper-container-horizontal" id="swiper_container">${temple_html_item}</div></div>'
  plus_style: ""

butterfly_article_double_row:
  enable: true

history_calendar:
  priority: 4
  enable: true
  enable_page: all
  layout:
    type: class
    name: sticky_layout
    index: 0
  temple_html: '<div class="card-widget card-history"><div class="card-content"><div class="item-headline"><i class="fas fa-clock fa-spin"></i><span>那年今日</span></div><div id="history-baidu" style="height: 100px;overflow: hidden"><div class="history_swiper-container" id="history-container" style="width: 100%;height: 100%"><div class="swiper-wrapper" id="history_container_wrapper" style="height:20px"></div></div></div></div>'

electric_clock:
  priority: 5
  enable: true
  enable_page: all
  layout:
    type: class
    name: sticky_layout
    index: 0
  temple_html: '<div class="card-widget card-clock"><div class="card-glass"><div class="card-background"><div class="card-content"><div id="hexo_electric_clock"><img id="card-clock-loading" src="https://cdn.jsdelivr.net/gh/Zfour/Butterfly-clock/clock/images/weather/loading.gif" style="height: 120px; width: 100%;" data-ll-status="loading" class="entered loading"></div></div></div></div></div>'
```
