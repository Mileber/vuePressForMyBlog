<template>
  <div class="article-card clearfix">
    <a class="cover-wrp" target="_blank" href="//www.bilibili.com/video/av18348303/">
      <img :src="imgUrl">
      <div class="duration">{{duration}}</div>
    </a>
    <div class="meta-wrp">
      <div class="meta-title">
        <span class="typename">{{tag}}</span>
        <a class="name ellipsis" target="_blank" href="//www.bilibili.com/video/av18348303/">{{title}}</a>
      </div>
      <div class="meta-status">
        <span class="pubdate">{{pubdate}}</span>
      </div>
    </div>
  </div>
</template>
<style scoped>
.cover-wrp {
  position: relative;
  float: left;
  width: 160px;
  height: 100px;
  border-radius: 4px;
  overflow: hidden;
  margin-right: 20px;
  background: #f1f3f7;
}
.article-card {
  position: relative;
  min-height: 100px;
  border-radius: 4px;
  background: #fff;
  box-shadow: 0.5px 1px 1px 2px #dfe5ed;
  margin: 20px;
  padding: 20px;
}
.duration {
  position: absolute;
  bottom: 0;
  right: 0;
  height: 20px;
  line-height: 20px;
  padding: 0 4px;
  background: rgba(0,0,0,.6);
  color: #fff;
  border-radius: 4px;
  font-size: 12px;
}
.meta-wrp {
  float: left;
}
.meta-title {
  height: 24px;
  line-height: 24px;
}
.name {
  display: inline-block;
  max-width: 460px;
  font-size: 18px;
  color: #212121;
}
.ellipsis {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.meta-status {
  padding: 18px 0 20px;
}
.pubdate {
  display: inline-block;
  color: #99a2aa;
  font-weight: 400;
  padding-right: 20px;
  border: none;
  vertical-align: middle;
  font-size: 14px;
}
.typename {
  display: inline-block;
  padding: 0 8px;
  border: 1px solid #e5e9ef;
  color: #666;
  border-radius: 12px;
  vertical-align: top;
  line-height: 22px;
  margin-right: 10px;
  font-size: 12px;
}
.meta-title a:hover {
  text-decoration-line: none;
  color: #ffc3ce;
}
</style>
<script>
export default {
  data () {
    return {

    }
  },
  props: ['imgUrl', 'duration', 'title', 'tag', 'pubdate']
}
</script>
