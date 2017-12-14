<template>
    <div id="contact">
        <a href="#about_me" class="title animated bounceIn">
            <p class="headline" id="about_me">About me</p>
        </a>
        <div class="info animated tada">
            <img src="../../../static/me.jpg" alt="me"/>
            <div class="wraper">
                <p class="left">邮箱:</p><p class="right">1255394075@qq.com</p>
                <p class="left">学校:</p><p class="right">电子科技大学成都学院计算机系</p>
                <p class="left">专业:</p><p class="right">计算机应用技术</p>
                <p class="left">姓名+学号:</p><p class="right">刘巧+1630610109</p>
                <p class="left">随笔感悟:</p><a class="right" href="http://loveqiao.top/">http://loveqiao.top/</a>
            </div>
        </div>
    </div>
</template>

<script>
import {mapMutations} from 'vuex'
export default {
    created () {
        this.set_headline({
            content: '关于我',
            animation: 'animated bounce'
        })
    },
    methods: mapMutations(['set_headline'])
}

</script>

<style lang="scss" rel="stylesheet/scss" scoped>
#contact {
    min-height: 30rem;
    padding: 0 1rem 5rem;
    background:#ffffff;
    align-content: center;
    .title {
        p.headline {
            width: 13rem;
        }
    }
    .info {
        position: relative;
        width: 55%;
        margin: 6.875rem auto 0;
        padding-bottom: 2rem;
        border: 0.1875rem solid pink;
        transition: all 2s;
        &:hover {
             background: pink;
             transition: all 2s;
         }
        img {
            width: 9.375rem;
            height: 9.375rem;
            border: 0.1875rem solid #cccccc;
            border-radius: 50%;
            position: absolute;
            left: 50%;
            margin-left: -4.6875rem;
            margin-top: -4.6875rem;
        }
        div.wraper {
            margin-top: 8.125rem;
            padding-left: 2rem;
            margin-left: 50px;
            p {
                display: inline-block;
                font-size: 1.25rem;
                color: #000000;
                margin-bottom: 1.5625rem;
            }
            .left {
                width: 30%;
                color: #000000;
            }
            .right {
                width: 50%;
                color: #000000;
            }
        }
    }
}
p.headline {
    padding-top: 4.375rem;
    margin: 0 auto 1.25rem;
    text-align: center;
    color: #000000;
    font-size: 2rem;
    padding-bottom: 1.25rem;
    border-bottom: 0.3125rem double pink;
}
@media screen and (max-width: 440px) {
    /*.title, .info {*/
        /*display: block !important;*/
    /*}*/
    .info {
        width: 100% !important;
    }
    .wraper {
        padding-left: 1rem !important;
        p {
            display: block !important;
        }
        p.left {
            color:#000000 !important;
        }
        p.right {
            width: 100% !important;
            color: #000000;
        }
    }
}
</style>
