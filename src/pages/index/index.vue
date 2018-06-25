<template>
    <div class="template">
        <searchBar></searchBar>
        <swiperBar></swiperBar>
    </div>
</template>

<script>
import card from '@/components/card'
import swiperBar from '@/components/home/swiper-bar'
import searchBar from '@/components/home/search-bar'

export default {
    data () {
        return {
            motto: 'Hello World',
            userInfo: {}
        }
    },

    components: {
        card,
        swiperBar,
        searchBar
    },

    methods: {
        bindViewTap () {
            const url = '../logs/main'
            wx.navigateTo({ url })
        },
        getUserInfo () {
            // 调用登录接口
            wx.login({
                success: () => {
                    wx.getUserInfo({
                        success: (res) => {
                            this.userInfo = res.userInfo
                        }
                    })
                }
            })
        },
        clickHandle (msg, ev) {
            console.log('clickHandle:', msg, ev)
        }
    },

    created () {
    // 调用应用实例的方法获取全局数据
        // this.getUserInfo()
    }
}
</script>

<style lang="scss" scoped>
    @import "../../style/variable";  
</style>
