<template>
  <div class="wcImglab">
    <div class="header"></div>
    <div class="mainBody"></div>
    <div class="imgSwiper">
      <imgSwiper></imgSwiper>
    </div>
  </div>
</template>

<script>
import imgSwiper from '@/components/imgSwiper'
export default {
  components:{
    imgSwiper
  }
}
</script>

<style >
  .wcImglab{
    /* display: flex;
    flex-direction:column; */
  }
  .header{
    width: 100%;
    height:50px;
    border-bottom: 2px solid red;
  }
  .mainBody{
    width: 100%;
    height: 430px;
    border-bottom: 2px solid red;
    
  }
</style>
