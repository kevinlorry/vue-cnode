<template>
  <div class="head">
    <div class="logo">
      <img src="../../assets/logo.svg"/>
    </div>
    <div class="search">
      <form method="get" action="http://www.baidu.com/s">
        <input type="text" class="searchInput" name="wd" autocomplete="off" />
      </form>
    </div>
    <div class="lead">
      <ul>
        <li> 首页</li>
        <li> 入门</li>
        <li> API</li>
        <li> 关于</li>
        <li> 注册</li>
        <li> 登陆</li>

      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss">
  .head{
    width:100%;
    background-color: #444;
    margin: 0 auto;
    text-align:center;
    .logo {
      img {
        width: 30%;
      }
      padding-top:10px;
    }
    .search{
      .searchInput{
        height: 25px;
        border-radius: 25px;
        width: 60%;
        padding-left: 22px;
        background: url("../../assets/search.png") 1px 3px no-repeat #888;
        &:hover{
          background-color: white;
        }
      }
    }
    .lead{
      /*height: 30px;*/
      li{
        display: inline-block;
        width: 15%;
        color:white;
        padding:10px 0 ;
        &:hover{
          opacity: 0.3;
        }
      }
    }
  }

</style>
