<template>
    <div class = 'new-course'>
        <div class = 'new-course-main'>
            <div class = 'new-course-t'>
                <div class='title-hot'>
                    <div class='hot'>Hot</div>
                    <div class="hot-c"></div>
                </div>
                <div class='title-text'>
                    <div class="txt">上新</div>
                </div>
               
            </div>
            
            <div class = 'new-course-header-b'>
                <ul class='new-course-b'>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                    <li>
                        <img src="@\assets\img\Backgd.jpg">
                        <div class="course-content">
                            <h3 >标题</h3>
                            <div>级别显示</div>
                            <div class="price">
                                <div class="price-vip">价格</div>
                                <div class="price-number">具体数字</div>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
.new-course-main{
    width: 1000px;
    margin: 0 auto;
}
.new-course-t{
    display: flex;
}
.title-hot{
    display: flex;
}
.title-hot .hot{
    width: 65px;
    line-height: 25px;
    text-align: center;
    color:aliceblue;
    background: #ff0000;
    border-radius: 5px 0px 5px 5px;
}
.title-hot .hot-c{
    width: 0px;
    height: 0px;
    border: 3px solid #ff0000;
    border-bottom-color: transparent;
    border-right-color: transparent;
}
.title-text{
    position: relative;
    margin-left: 5px ;
    line-height: 25px;
    font-size:25px;
    color: #333333;
}
.title-text :after{
    position: absolute;
    content:"";
    left: 0;
    bottom: 0;
    z-index: -1;
    width:140%;
    height: 9px;
    margin-left: -20%;
    background-color: #4184d1;
    border-radius:5px;
}

.new-course-b{
    display:flex;
    justify-content: space-between;
    
    flex-wrap: wrap; /* 允许列表项换行 */
}
/* .new-course-b >li{
    display: inline-block;
} */
.new-course-b li{
    display:flex;
    flex-direction: column;
    align-items: center;
    width: 240px;
    height: 275px;
    background-color: rgb(244, 241, 237);
    box-shadow:1px,3px,3px rgba(27,39,94,0.1);
    opacity:1;
    border-radius: 5px;
    margin-top: 15px;

}
.new-course-b li img{
    padding-top: 5%;
    width: 90%;
    
}
.course-content{
    width: 90%;
    
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    height: 120px;
}

.course-content h3{
    font-size:15px;
}
.course-content >div{
    font-size: 12px;
}
.price{
    display: flex;
}
.price-vip{
    background: linear-gradient(90deg,#FF928E 0%,#FFC17C 100%);
    border-radius: 16px 0px 16px 0px;
    text-align: center;
    width:64px;
    height: 16px;
    
}
.price-number{
    font-size: 12px;
    opacity: 1;
    color: #FF928E;
}
</style>