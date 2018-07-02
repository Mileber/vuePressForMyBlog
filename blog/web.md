---
title: 前端技术相关内容
lang: en-US
meta:
  - name: keywords
    content: blog javascript minecraft
footer: 三三的小狐狸
sidebarDepth: 2
---

## 分类/系列
<GroupLink v-for='g in groups' :link='g.link' :title='g.title' :imgUrl='g.imgUrl'/>

## 时间线
<ArticleLink v-for="a in articles" :link="a.link" :tag="a.tag" :title="a.title"/>

<script>
  export default {
    data () {
      return {
        groups:[
          {
            link: './web/100/list.html',
            title: '百题挑战',
            imgUrl: './../hero.jpg'
          },
          {
            link: '',
            title: 'Vue相关',
            imgUrl: './../hero.jpg'
          },
          {
            link: '',
            title: '其他',
            imgUrl: './../hero.jpg'
          }
        ],
        articles:[
          {
            link: './web/100/012.html',
            tag: '百题挑战',
            title: '012-The observed PIN',
          },
          {
            link: './web/100/011.html',
            tag: '百题挑战',
            title: '011-Strings Mix'
          }
        ]
      }
    }
  }
</script>