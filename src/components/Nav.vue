<template>
    <div class="container clearfix nav" id="layout">
        <div class="fl nav-logo"></div>
        <ul class="fr nav-text">
            <li class="">
                <img src="./../assets/images/ticketsPC/person.png">
                <!-- <img src="~/images/ticketsPC/person.png" /> -->
                <router-link to="users">个人中心</router-link> |
            </li>
            <li class="">
                <span class="userPhone"></span>
            </li>
            <li class="login">
                <!-- <img src="~/images/ticketsPC/login1.png" width="22" height="22" /> -->
                <router-link to="login">登录</router-link>
            </li>
            <li class="register">
                <!-- <img src="~/images/ticketsPC/register.png" width="22" height="22" /> -->
                <router-link to="register">注册</router-link>
            </li>
            <li class="logout">
                <!-- <img src="~/images/ticketsPC/register.png" width="22" height="22" /> -->
                <span v-on:click="Logout()" style="cursor:pointer">退出</span>
            </li>
            <li>
                <!-- <img src="~/images/ticketsPC/goupiao.png" style="vertical-align:middle" /> -->
                <router-link to="tickets">购票</router-link>
            </li>
            <li onclick="window.location.href='http://www.baidu.com'" style="cursor:pointer">
                <!-- <img src="~/images/ticketsPC/return.png" style="vertical-align:middle" /> -->
                <a>返回 官网</a>
            </li>
        </ul>
    </div>

</template>
<script>
export default {
    name:'nav',
}
</script>
<style>
.nav {
    height: 60px;
    background: #fff;
    line-height: 60px;
    padding: 5px 10px;
}
.nav-logo { 
    width: 188px;
    height: 45px;
    background-image: url('./../assets/images/ticketsPC/galasysLogo.png');
    background-repeat: no-repeat;
    background-size: contain;
}

.nav-text li {
    float: left;
    margin-left: 54px;
    line-height: 50px
}

    .nav-text li img {
        vertical-align: text-bottom;
        margin-right: 10px;
    }
</style>