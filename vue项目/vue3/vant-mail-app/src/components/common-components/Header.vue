<template>
  <div class="header">
    <van-nav-bar title="标题" left-text="返回" left-arrow   @click-left="goBack">
      <!-- <van-icon name="search" size="16px" slot="right"/> -->
    </van-nav-bar>
  </div>
</template>
<script>
export default {
  name: "Header",
  data () {
    return {
      
    }
  },
  methods: {
    goBack () {
      this.$router.go(-1);
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .header{
    width: 100%;
  }
  .van-hairline--bottom::after {
     border-bottom-width: 0px; 
  }
  .van-nav-bar{
    background: #1989fa;
  }
  .van-nav-bar .van-icon{
    color: #fff;
  }
  .van-nav-bar__title{
    color: #fff;
  }
  .van-nav-bar__text{
    color:#fff;
  }
</style>
