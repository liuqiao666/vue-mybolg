<template>
    <div>
        <a href="#" class="iconfont icon-iconsf"></a>
        <a class="iconfont icon-github" href="https://github.com/liuqiao666"></a>
        <a href="#" class="iconfont icon-cion15"></a>
        <p>学号：1630610109</p>
        <p>Copyright @ 2017 Powered by Vue. Designed by liuqiao | <router-link :to="{name: 'login'}" tag="span" class="login">站长登录</router-link></p>
    </div>
</template>

<script>
export default {}

</script>

<style lang="scss" rel="stylesheet/scss" scoped>
    .iconfont {
       font-size: 1.875rem;
       color: #fff;
       margin-right: 0.625rem;
    }
    .icon-github:hover {
             color: royalblue;
    }
    .icon-cion15 {
        font-size: 1.625rem;
    }
    .icon-cion15:hover {
        color: deepskyblue;
    }
    .icon-iconsf:hover {
        color: green;
    }
    div {
        text-align: center;
        padding-top: 0.625rem;
        line-height: 2.5rem;
        width: 100%;
        background: #111111;
    }
    p {
        text-align: center;
        color: #ffffff;
        font-size: 1rem;
    }
    span.login {
        cursor: pointer;
        color: #fff;
    }
</style>
