<template>
 <div  class="header-container">
     <div class="left-block">
         <el-image round style="width: 60px; height: 60px" src="https://fuss10.elemecdn.com/e/5d/4a731a90594a4af544c0c25941171jpeg.jpeg" fit="cover"></el-image>
         深圳橙鹿设计顾问有限责任公司
     </div>
     <div class="right-block">
         <!-- 导航部分 -->
     </div>
 </div>
</template>

<script>
 export default {
  name: '',
  data () {
   return {

   }
  },
  components: {

  }
 }
</script>

<style lang="less" scoped>
.header-container{
    width: 100%;
    height:80px;
    background-color: #ffffff;
    position: fixed;
    top: 0px;
    left: 0px;
    z-index:99;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .left-block{
        display: flex;
        align-items: center;
        font-size: 24px;
        color: #FF6600;
        font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

    }
}
</style>
