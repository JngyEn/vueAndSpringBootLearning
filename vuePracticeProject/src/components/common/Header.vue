<template>
    <header>
        <div class='header-main'>
            <div class="header-l">
                <h1 class="logo">
                    <img src = "@/assets/img/图片1.jpg" />

                </h1>
                <ul>
                    <li class="active">首页</li>
                    <li>课程</li>
                    <li>会员</li>
                </ul>
            </div>

            <div class="header-r">
                <div class='search'>
                    <input type = "" placeholder="搜索课程" />
                    <el-icon :size="20"><Search /></el-icon>
                </div>
                <div class="shop">
                    <el-icon :size="20"><ShoppingCart /></el-icon>
                </div>
                <div class="login">
                    登录/注册
                </div>

            </div>
        </div>
    </header>
</template>

<script setup>
import { Search ,ShoppingCart} from '@element-plus/icons-vue';

</script>

<style scoped>
header{
    width:100%;
    height:100px;
}
.header-main{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width:1000px;
    height: 100%;
    margin:0 auto;

}

.header-l {
    display:flex;
    justify-content: space-between;
    align-items: center;
    
}
.logo{
    width:120PX;
    height:90%;
    margin-right: 51px;
}
.logo img{
    width:80%;
    height:80%;
}
.header-l ul{
    display:flex;
    height: 50px;
}
.header-l ul li{
    line-height: 50px;
    font-weight: 600;
    cursor:pointer;
}
.header-l ul li+li{
    margin-left: 79PX;
    font-size:16px;
    color: #808080;
    line-height: 50px;
    font-weight: 300;
}

.header-r {
    display:flex;
    justify-content: space-between;
    align-items: center;
}

.header-r .search{
   display: flex;
   align-items: center;
   padding: 0 10px;
   width:300px;
   height: 43px;
   background: #a5a7a947;
   border-radius: 5PX;
}

.header-r .search input{
   width: 270px;
   height: 43px;
   background:transparent;
   border: none;
   outline: none;
}
.header-r .shop{
    margin-left: 42px;
    align-items:center;
}
.header-r .login{
    margin-left: 39px;
    align-items:center;
    font-size:16px;
    cursor:pointer;
}
.active{
    position: relative;
}
.active:after{
    content:'';
    position: absolute;
    bottom: 0;
    left:0;
    width:140%;
    height:3px;
    background-color: #3585FF;
    margin-left:-12%;
}

</style>
