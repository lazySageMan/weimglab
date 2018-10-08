<template>
    <div>
        <swiper
            display-multiple-items="4"
        >
            <block :key="index" v-for="(item,index) in imgArr">
                <swiper-item class="swiper-item">
                    <image @click="getImgInfo(item,index)" :src="item" class="slide-image imgMargin" height="50"/>
                </swiper-item>
            </block>
        </swiper>
    </div>
</template>
<script>
import img1 from '../../static/img/1.jpg'
import img2 from '../../static/img/2.jpg'
import img3 from '../../static/img/3.jpg'
import img4 from '../../static/img/4.jpg'
import img5 from '../../static/img/5.jpg'
export default {
    data(){
        return {
           imgArr : [
               img1,
               img2,
               img3,
               img4,
               img5
           ] 
        }
    },
    methods:{
        getImgInfo(img,index){
            console.log(img)
            console.log(index)
        }
    }
}
</script>
<style>
    .imgMargin{
        margin:0 10rpx;
    }
    /* .imgMargin:first-child{
        margin-left: 0;
    } */
</style>


