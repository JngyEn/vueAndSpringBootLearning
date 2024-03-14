<template>
    <div class=" nav-swiper">
        <div class="nav-swiper__main">
            <div class = 'swipte-t'>
                <ul>
                    <li class="active">
                        <span>HTML/CSS</span>
                        <el-icon><ArrowRight /></el-icon>
                    </li>
                    <li>
                        <span>HTML/CSS</span>
                        <el-icon><ArrowRight /></el-icon>
                    </li>
                    <li>
                        <span>HTML/CSS</span>
                        <el-icon><ArrowRight /></el-icon>
                    </li>
                    <li>
                        <span>HTML/CSS</span>
                        <el-icon><ArrowRight /></el-icon>
                    </li>
                    <li>
                        <span>HTML/CSS</span>
                        <el-icon><ArrowRight /></el-icon>
                    </li>
                </ul>
                <div>
                    <el-carousel :interval="5000" arrow="always">
                    <el-carousel-item v-for="item in 4" :key="item">
                    <h3 text="2xl" justify="center">{{ item }}</h3>
                    </el-carousel-item>
                    </el-carousel>
                </div>
            </div>

            <ul class = 'swipte-b'>
                <li >
                    <h3>
                        <img src="@/assets/按钮/小红书.png" />
                    </h3>
                    <div>
                        <h4>初级课程</h4>
                        <span>乐</span>
                    </div>
                </li>
                <li>
                    <h3>
                        <img src="@/assets/按钮/小红书.png" />
                    </h3>
                    <div>
                        <h4>初级课程</h4>
                        <span>乐</span>
                    </div>
                </li>
                <li>
                    <h3>
                        <img src="@/assets/按钮/小红书.png" />
                    </h3>
                    <div>
                        <h4>初级课程</h4>
                        <span>乐</span>
                    </div>
                </li>
                <li>
                    <h3>
                        <img src="@/assets/按钮/小红书.png" />
                    </h3>
                    <div>
                        <h4>初级课程</h4>
                        <span>乐</span>
                    </div>
                </li>
                <li>
                    <h3>
                        <img src="@/assets/按钮/小红书.png" />
                    </h3>
                    <div>
                        <h4>初级课程</h4>
                        <span>乐</span>
                    </div>
                </li>
                
            </ul>
        </div>
    </div>
</template>

<script setup>
import { ArrowRight } from '@element-plus/icons-vue';
</script>

<style scoped>
.nav-swiper{
    background: url('@/assets/img/Backgd.jpg') no-repeat;
    width: 100%;
    height: 600px;
}
.nav-swiper__main{
    display: flex;
    flex-direction: column; 
    align-self: center;
    width: 1000px;
    height: 600px;
    margin: 0 auto;
    padding: 47px 0;
}
.swipte-t{
    display: flex;
    height: 373px;
    opacity: 1;
    border-radius: 11px 11px 0px 0px;
}
.swipte-t ul{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    height: 100%;
    width: 160px;
    background-color: #2B283D;
    border-radius: 11px 0px 0px 0px;

}
.swipte-t ul li{
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 160px;
    height:37px;
    font-size:16px;
    color: #F2F2F2;
    cursor: pointer;
}
.active{
    background: linear-gradient(to right, 
                            rgba(25, 85, 123, 1) 0%, 
                            rgba(25, 85, 123, 0.9) 10%, 
                            rgba(25, 85, 123, 0.8) 20%, 
                            rgba(25, 85, 123, 0.7) 30%, 
                            rgba(25, 85, 123, 0.6) 40%, 
                            rgba(25, 85, 123, 0.5) 50%, 
                            rgba(25, 85, 123, 0.4) 60%, 
                            rgba(25, 85, 123, 0.3) 70%, 
                            rgba(25, 85, 123, 0.2) 80%, 
                            rgba(25, 85, 123, 0.1) 90%, 
                            rgba(0, 0, 0, 0) 100%);


}
.swipte-t > div{
    height: 373px;
    width: 840px;
}

.el-carousel {
    height: 373px;
}
::v-deep .el-carousel__container{
    height: 373px;
}

.swipte-b{
    display: flex;
}
.swipte-b li{
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 213px;
    height: 133px;
    background-color: #FFFFFF;
    border-radius: 0px 0px 11px 11px;
    text-align: center;
    cursor: pointer;
}
.swipte-b li img{
    width: 64px;
    height: 64px;
    background-color: #FFFFFF;
    border-radius: 11px 11px 11px 11px;
}
.swipte-b li div{
    margin-left: 11px;
}
.swipte-b li div h4{
    font-size: 16px;
    color: #333333;
}
.swipte-b li div span{
    font-size: 12px;
    color: #808080;
}
</style>