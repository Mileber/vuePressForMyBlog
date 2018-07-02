<template>
  <div class="article-card clearfix">
    <a class="cover-wrp" target="_blank" :href="link">
      <img :src="imgUrl">
    </a>
    <div class="meta-wrp">
      <div class="meta-title">
        <a class="name ellipsis" target="_blank" :href="link">{{title}}</a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {

    }
  },
  props: ['imgUrl', 'link', 'title']
}
</script>
<style scoped>
.article-card {
  position: relative;
  height: 150px;
  border-radius: 4px;
  background: #fff;
  box-shadow: 0.5px 1px 1px 2px #dfe5ed;
  margin: 20px;
  padding: 20px;
  display: inline-block;
  vertical-align: top;
  width: 165px;
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
