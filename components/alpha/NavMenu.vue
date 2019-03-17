<template>
    <div class="nav-wrap">
      <div class="nav">
        <div class="mask"></div>
        <div class="menu alpha-wrap">
          <div class="left">
            <ul>
              <li>栏目1</li>
              <li>栏目2</li>
              <li>栏目3</li>
              <li>栏目4</li>
              <li>栏目5</li>
            </ul>
          </div>
          <div class="right">q</div>
        </div>
      </div>
      <div class="banner"></div>
    </div>
</template>

<script>
  export default {
    name: 'NavMenu',
    data(){
      return {

      }
    }
  }
</script>

<style lang="less">
.nav-wrap{
  .nav{
    position: relative;
    height: 42px;
    background-color: hsla(0,0%,100%,.4);
    box-shadow: 0 1px 2px rgba(0,0,0,.1);
    z-index: 200;
  }
  .mask{
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    filter: blur(4px);
    background-position: center -10px;
    background-repeat: no-repeat;
    background-image:url("../../assets/bg.png");
  }
  .menu{
    position: relative;
    display: flex;
    justify-content: space-between;
  }
  .left{
    ul{
      display: flex;
    }
    li{
      flex: 1;
      color: #222;
      font-size: 12px;
      padding: 0 10px;
      line-height: 42px;
      white-space: nowrap;
    }
  }
  .banner{
    position: relative;
    height: 170px;
    margin-top: -42px;
    background:url("../../assets/bg.png") no-repeat;
    z-index: 100;
  }
}
</style>
