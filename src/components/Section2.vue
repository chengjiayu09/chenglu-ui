<template>
 <div  class="container">
     <h3>经典案例</h3>
     <div class="content-block">
          <el-image :src="imgCase3" lazy></el-image>
        <el-row>
            <el-col :span="12">
                <el-carousel trigger="click" height="350px">
                    <el-carousel-item v-for="item in list" :key="item.title">
                        <img :src="item.url" hieght="200px" model="cover"/>
                    </el-carousel-item>
                </el-carousel>
            </el-col>
            <el-col :span="12"><div class="grid-content bg-purple-light"></div></el-col>
        </el-row>
     </div>
 </div>
</template>

<script>
import imgCase1 from "@/assets/images/case1.png";
import imgCase2 from "@/assets/images/case2.png";
import imgCase3 from "@/assets/images/case3.png";
 export default {
  name: 'Section2',
  data () {
   return {
       imgCase3,
       list:[
           {url:imgCase1,title:'案例一',desc:'这是一个幼儿园项目'},
           {url:imgCase2,title:'案例二',desc:'这是第二个幼儿园项目'},
           {url:imgCase3,title:'案例三',desc:'这是第三个幼儿园项目'},
           {url:imgCase2,title:'案例四',desc:'这是第四个幼儿园项目'},
       ]
   }
  },
  components: {

  }
 }
</script>

<style lang="less" scoped>
.carousel-block{

}
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 150px;
  margin: 0;
}
.el-carousel__item {
   background-color: #99a9bf;
   img{
       object-fit: cover;
   }
}
</style>
