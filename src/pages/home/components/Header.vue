<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/主题
    </div>
    <router-link to="/city">
      <div class="header-right">
        {{this.$store.state.city}}
        <span class="iconfont arrow-icon">&#xe64a;</span>
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
@import '~@/commons/styles/index.styl'
.header{
  line-height: $header-height;
  display: flex;
  background-color: $bg-color;
  font-size: .3rem;
  color: #fff;
  .header-left{
    width: .86rem;
    float: left;
    .back-icon{
      text-align: center;
      font-size: .4rem;
    }
  }
  .header-input{
    padding-left: .2rem;
    flex: 1;
    height: .64rem;
    line-height: .64rem;
    margin-top: .12rem;
    margin-left: .2rem;
    background-color: #fff;
    border-radius: .1rem;
    color: #ccc;
  }
  .header-right{
    width: 1.24rem;
    float: right;
    text-align: center;
    color: #fff;
    no-wrap();
    .arrow-icon{
      margin-left: -.08rem;
      font-size: .24rem;
    }
  }
}
</style>
