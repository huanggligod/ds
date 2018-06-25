<!-- search-bar -->
<template>
    <div>
        <div class="search-bar">
            <icon class="home" color="white" @tap="routeToHome" />
            <span class="text">请输入搜索内容...</span>
            <div class="cs-box">
                <icon class="chat" color="white" />
                <text class="cs-txt">咨询</text>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'searchBar',
    data () {
        return {
        }
    }
}
</script>
<style lang='scss' scoped>
    @import "../../style/icons";
    .search-bar {
        background: $color-primary;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 40px;

        .home {
            width: 35px;
        }
        .text {
            width: 260px;
            font-size: 12px;
            color: $color-muted;
            background: #fff;
            padding: 4px 14px;
            box-sizing: border-box;
           border-radius: 3px;
        }
        .cs-box {
            flex: 1;
            height: 40px;
            display: flex;
            justify-content: center;
            align-items: center;

            .chat {
                margin-top: 3px;
            }

            .cs-txt {
                font-size: 14px;
                color: #fff;
            }
        }
    }
</style>