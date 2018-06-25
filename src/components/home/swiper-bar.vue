<!-- swiper-bar -->
<template>
    <div class="swiper-bar">
        <swiper class="swiper" indicator-dots="true" indicator-active-color="#eee" interval="3000" circular="true" autoplay="true">
            <swiper-item>
                <image mode="aspectFit" src="http://img.leshare.shop/shop/3/swiper_1.jpg"></image>
            </swiper-item>
            <swiper-item>
                <image mode="aspectFit" src="http://img.leshare.shop/shop/3/swiper_2.jpg"></image>
            </swiper-item>
            <swiper-item>
                <image mode="aspectFit" src="http://img.leshare.shop/shop/3/swiper_3.jpg"></image>
            </swiper-item>
        </swiper>
    </div>
</template>

<script>
export default{
    name: 'swiperBar',
    data () {
        return {
        }
    }
}
</script>

<style lang='scss' scoped>
    .swiper {
        width: 100%;
        height: 117px;

        image {
            width: 100%;
            height: 100%;
        }
    }

</style>
