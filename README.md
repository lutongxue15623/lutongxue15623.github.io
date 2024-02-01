<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        *{
            margin: 0px;
            padding: 0px;
        }
        ul li{
            list-style: none;
        }
        a{
            color: #ffffff;
            text-decoration: none;
        }
        body{
            background-color: #f5efe5;
            font-size: 12px;
            font-family: 'microsoft yahei', Araial;
        }
        #header{
            width: 100%;
            height: 90px;
            background-image: url(img/background.png);
        }
        #header .top{
            width: 1002px;
            height: 90px;
            margin: 0px auto;
            position: relative;
        }
        #header .top .logo img{
            width: 235px;
            position: relative;
            top: 10px;
            left: 10px;
        }
        #header .top .service{
            width: 60px;
            height: 20px;
            position: absolute;
            right: 5px;
            top: 10px;
        }
        #header .top .service ul{
            position: absolute;
            top: 20px;
            right: 7px;
            z-index: 5;
            display: none;
        }
        #header .top .service ul li{
            width: 60px;
            height: 20px;
            background-color: #011648;
            background-image: none;
        }
        #header .top .service:hover ul{
            display: block;
        }
        #header .top .service a span{
            width: 0px;
            height: 0px;
            border: 5px solid transparent;
            border-top: 5px solid #ffffff;
            margin-left: 3px;
            position: relative;
            top: 12px;
        }
        #header .top ul{
            position: absolute;
            right: 200px;
            bottom: 10px;
        }
        #header .top ul li{
            width: 63px;
            height: 16px;
            float: left;
            text-align: center;
            line-height: 16px;
            background-image: url(img/li1.gif);
            background-position: 0px 2px;
            background-repeat: no-repeat;
        }
        #header .top .search-box{
             width: 174px;
             height: 29px;
             background-color: #ffffff;
             position: absolute;
             right: 10px;
             bottom: 5px;
             border-radius: 10px;
        }
        #header .top .search-box input{
            width: 126px;
            height: 16px;
            margin-right: 15px;
            position: relative;
            top: -10px;
            left: 15px;
            border: none;
            outline: 0;
            font-size: 12px;
            color: #666;
        }
        #header .top a:hover{
            color: #066;
        }
        #main{
            width: 100%;
            height: 625px;
            background-image: url(img/bjtpchun.jpg);
            background-position: 50% 37px;
            background-repeat: no-repeat;
        }
        #main .nav{
            width: 100%;
            height: 37px;
            background: url(img/background.png) 0px -90px repeat-x;
            position: relative;
            z-index: 2;
        }
        #main .nav ul{
            width: 981px;
            height: 37px;
            margin: 0px auto;
            display: flex;
        }
        #main .nav ul li{
            flex: 1;
            height: 37px;
            text-align: center;
            line-height: 37px;
        }
        #main .nav ul li a{
            font-size: 15px;
        }
        #main .nav ul li div{
            position: relative;
            top: -1px;
            display: none;
            width: 100%;
        }
        #main .nav ul li div a{
            width: 100%;
            height: 19px;
            background: url(img/background.png) 0px -800px;
            font-size: 12px;
            line-height: 19px;
            display: block;
            text-align: left;
            padding-left: 10px;
        }
        #main .nav ul li div a:hover{
            background: url(img/background.png) 0px -780px;
            color: #e58100;
        }
        #main .nav ul li:hover{
            background: url(img/background.png) 0px -820px;
        }
        #main .nav ul li:hover div{
            display: block;
        }
        #main .news{
            width: 988px;
            height: 626px;
            margin: 0px auto;
            position: relative;
            z-index: 1;
        }
        #main .news .news_main{
            width: 988px;
            height: 570px;
            background-image: url(img/0533e885-0901-4cee-897b-f2e49b5d88fe.jpeg);
            background-size: 100%;
            position: absolute;
            top: -35px;
            z-index: 2;
        }
        #main .news .news_main .news_main_left{
            width: 25px;
            height: 64px;
            background: url(img/carousel-nav.png);
            position: absolute;
            left: -30px;
            top: 250px;
        }
        #main .news .news_main .news_main_left a{
            width: 25px;
            height: 64px;
            display: block;
        }
        #main .news .news_main .news_main_left:hover{
            background: url(img/carousel-nav.png) left bottom;
        }
        #main .news .news_main .news_main_right{
            width: 25px;
            height: 64px;
            background: url(img/carousel-nav.png) right top;
            position: absolute;
            right: -30px;
            top: 250px;
        }
        #main .news .news_main .news_main_right:hover{
            background: url(img/carousel-nav.png) right bottom;
        }
        #main .news .news_main .news_main_right a{
            width: 25px;
            height: 64px;
            display: block;
        }
        #main .news .news_main p{  
            display: inline-block;
            width: 361px;
            height: 35px;
            font-size: 14px;
            line-height: 35px;
            text-align: center;
            background-image: url(img/ban_tit_bg.png);
            position: relative;
            top: 410px;
            left: 10px;
        }
        #main .news .news_main .hot{
            width: 341px;
            height: 426px;
            position: absolute;
            top: 50px;
            right: 35px;
            background: url(img/news_bg.png);
        }
        #main .news .news_main .hot .hot_top{
            width: 341px;
            height: 5px;
            background: url(img/background.png) 0px -864px ;
        }
        #main .news .news_main .hot .hot_middle{
            width: 305px;
            height: 198px;
            background: #e58100;
            margin: 0px auto;
            position: relative;
        }
        #main .news .news_main .hot .hot_middle ul{
            position: absolute;
            top: 5px;
            left: 10px;
        }
        #main .news .news_main .hot .hot_middle ul li{
            float: left;
            width: 64px;
            height: 20px;
            margin-left: 5px;
            text-align: center;
            line-height: 20px;
            background-color: #c26e02;
        }
        #main .news .news_main .hot .hot_middle ul li:nth-child(1){
            background-color: #905302;
        }
        #main .news .news_main .hot .hot_middle ul li:hover{
            background-color: #905302;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img{
            width: 275px;
            height: 155px;
            position: relative;
            top: 30px;
            left: 15px;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img a img{
            width: 100%;
            height: 100%;
            position: relative;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img .hot_middle_img_a{
            width: 275px;
            height: 30px;
            display: block;
            background: url(img/background.png) 0px -409px;
            line-height: 30px;
            position: absolute;
            bottom: 0px;
            color: #e58100;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img .hot_middle_img_a span{
            margin-left: 3px;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img .hot_middle_img_a:hover{
            color: #c60;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img ul{
            position: absolute;
            left: 232px;
            top: 138px;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img ul li{
            width: 7px;
            height: 7px;
            margin-left: 3px;
            background: url(img/background.png) -277px -449px;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img ul a:nth-child(1) li{
            background: url(img/background.png) -285px -449px;
        }
        #main .news .news_main .hot .hot_middle .hot_middle_img ul li:hover{
            background: url(img/background.png) -285px -449px;
        }
        #main .news .news_main .hot .hot_bottom{
            width: 305px;
            height: 217px;
            background: url(img/news_bg_1.jpg) #ac6304 repeat-x;
            margin: 0px auto;
            position: relative;
        }
        #main .news .news_main .hot .hot_bottom div{
            position: absolute;
            top: 5px;
            left: 15px;
        }
        #main .news .news_main .hot .hot_bottom div span{
            width: 40px;
            height: 20px;
            background-color: #c26e02;
            float: left;
            margin-right: 5px;
            text-align: center;
            line-height: 20px;
        }
        #main .news .news_main .hot .hot_bottom div span:nth-child(1){
            background-color: #e58100;
        }
        #main .news .news_main .hot .hot_bottom div span:hover{
            background-color: #e58100;
        }
        #main .news .news_main .hot .hot_bottom ul{
            position: absolute;
            top: 30px;
            left: 17px;
        }
        #main .news .news_main .hot .hot_bottom ul li{
            width: 269px;
            height: 21px;
            background: url(img/background.png) 0px -370px repeat-x;
        }
        #main .news .news_main .hot .hot_bottom ul h4{
            width: 269;
            text-align: right;
            font-weight: normal;
        }
        #main .news .news_main .hot .hot_bottom ul a:hover{
            color: #066;
        }
        #main .news .news_main .hot .hot_bottom_i1{
            width: 341px;
            height: 9px;
            background: url(img/news_bottom_bg.png);
        }
        #main .news .news_main .column{
            width: 988px;
            height: 46px;
            background: url(img/background.png) 0px -402px;
            position: absolute;
            bottom: 0px;
        }
        #main .news .news_main .column ul{
            width: 756px;
            height: 39px;
            display: flex;
            flex-wrap: wrap;
            padding-top: 6px;
            padding-left: 20px;
        }
        #main .news .news_main .column ul li{
            width: 150px;
            height: 16px;
            background: url(img/background.png) -334px -238px no-repeat; 
            line-height: 16px;
        }
        #main .news .news_main .column ul li a{
            margin-left: 20px;
            color: #e58100;
            font-size: 15px;
        }
        #main .news .news_footer{
            width: 988px;
            height: 53px;
            background-color: #011648;
            position: absolute;
            bottom: 38px;
        }
        #main .news .news_footer a{
            text-decoration: underline;
        }
        #main .news .news_footer a:hover{
            color: #066;
        }
        #main .news .news_footer .news_footer_left{
            width: 740px;
            height: 36px;
            padding: 10px 20px;
            color: #ffffff;
            position: relative;
        }
        #main .news .news_footer .news_footer_left ul{
            display: flex;
            position: absolute;
            right: 5px;
            top: 10px;
        }
        #main .news .news_footer .news_footer_left ul li{
            width: 27px;
            height: 27px;
            margin-right: 5px;
        }
        #main .news .news_footer .news_footer_left ul li a{
            width: 27px;
            height: 27px;
            display: block;
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(1){
            background: url(img/sns_icons2.png);
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(2){
            background: url(img/sns_icons2.png) -27px 0px ;
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(3){
            background: url(img/sns_icons2.png) -56px 0px ;
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(4){
            background: url(img/sns_icons2.png) -88px 0px ;
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(1):hover{
            background: url(img/sns_icons2.png) 0px -30px;
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(2):hover{
            background: url(img/sns_icons2.png) -27px -30px;
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(3):hover{
            background: url(img/sns_icons2.png) -56px -30px;
        }
        #main .news .news_footer .news_footer_left ul li:nth-child(4):hover{
            background: url(img/sns_icons2.png) -88px -30px;
        }
        #main .news .news_footer .news_footer_right{
            position: absolute;
            right: 15px;
            top: 17px;
        }
    </style>
</head>
<body>
    <div id="header">
        <div class="top">
            <div class="logo"><a href="#"><img src="img/logo (1).png" alt=""></a></div>
            <div class="service">
                <a href="#">English<span></span></a>
                <ul>
                    <li><a href="#">Russisch</a></li>
                    <li><a href="#">Deutsch</a></li>
                </ul>
            </div>
            <ul>
                <li><a href="#">信息公开</a></li>
                <li><a href="#">校园导航</a></li>
                <li><a href="#">浙大服务</a></li>
            </ul>
            <div class="search-box"><input type="text" placeholder="浙大百事通搜索"><a href="#"><img src="img/main-logo.png" alt=""></a></div>
        </div>
    </div>
    <div id="main">
        <div class="nav">
            <ul>
                <li>
                    <a href="Overview.html" target="_parent">校园总览</a>
                    <div>
                        <a href="#">学校概况</a>
                        <a href="#">学校章程</a>
                        <a href="#">学校标识</a>
                        <a href="#">现任领导</a>
                        <a href="#">统计公报</a>
                        <a href="#">虚拟校园</a>
                        <a href="#">校史馆</a>
                    </div>
                </li>
                <li><a href="#">求是新闻</a></li>
                <li><a href="#">综合服务</a></li>
                <li>
                    <a href="#">学校机构</a>
                    <div>
                        <a href="#">党群机构</a>
                        <a href="#">行政机构</a>
                        <a href="#">学术机构</a>
                        <a href="#">学院（系）</a>
                        <a href="#">附属医院</a>
                        <a href="#">校区</a>
                        <a href="#">直属单位</a>
                        <a href="#">全国重点实验室</a>
                        <a href="#">有关企业</a>
                        <a href="#">校设研究机构</a>
                    </div>
                </li>
                <li>
                    <a href="#">教师队伍</a>
                    <div>
                        <a href="#">两院院士</a>
                        <a href="#">文科资深教授</a>
                        <a href="#">教育部教学名师</a>
                        <a href="#">教师个人主页</a>
                    </div>
                </li>
                <li>
                    <a href="#">教育教学</a>
                    <div>
                        <a href="#">本科教育</a>
                        <a href="#">研究生教育</a>
                        <a href="#">国际教育</a>
                        <a href="#">继续教育</a>
                    </div>
                </li>
                <li>
                    <a href="#">科学研究</a>
                    <div>
                        <a href="#">科研基地</a>
                        <a href="#">科学技术研究院</a>
                        <a href="#">社会科学研究院</a>
                        <a href="#">工业技术转化研究院</a>
                        <a href="#">农业技术推广中心</a>
                        <a href="#">学术期刊</a>
                        <a href="#">科学封面</a>
                        <a href="#">科研政策专题</a>
                    </div>
                </li>
                <li>
                    <a href="#">招生就业</a>
                    <div>
                        <a href="#">本科生招生</a>
                        <a href="#">研究生招生</a>
                        <a href="#">国际学生招生</a>
                        <a href="#">就业指导服务</a>
                    </div>
                </li>
                <li>
                    <a href="#">校园生活</a>
                    <div>
                        <a href="#">浙江大学报</a>
                        <a href="#">学术资助</a>
                        <a href="#">体育与艺术</a>
                        <a href="#">浙大图库</a>
                        <a href="#">求是印象</a>
                        <a href="#">信息化服务</a>
                    </div>
                </li>
            </ul>
        </div>
        <div class="news">
            <div class="news_main">
                <div class="news_main_left"><a href="#"></a></div>
                <div class="news_main_right"><a href="#"></a></div>
                <a href="#"><p>科学头条|领域里程碑，超长寿命的钙钛矿LED在浙大诞生</p></a>
                <div class="hot">
                    <div class="hot_top"></div>
                    <div class="hot_middle">
                        <ul>
                            <li><a href="News.html" target="_blank">图片新闻</a></li>
                            <li><a href="#">视频新闻</a></li>
                        </ul>
                        <div class="hot_middle_img">
                            <a href="#"><img src="img/9c2989f0-8904-4cc0-b68a-5878b2c02e60_s.jpg" alt=""></a>
                            <a href="#" class="hot_middle_img_a"><span>浙江大学图书馆主馆试开馆</span></a>
                            <ul>
                                <a href="#"><li></li></a>
                                <a href="#"><li></li></a>
                                <a href="#"><li></li></a>
                                <a href="#"><li></li></a>
                            </ul>
                        </div>
                    </div>
                    <div class="hot_bottom">
                        <div>
                            <span><a href="#">新闻</a></span>
                            <span><a href="#">公告</a></span>
                            <span><a href="#">学术</a></span>
                            <span><a href="#">文体</a></span>
                            <span><a href="#">交流</a></span>
                        </div>
                        <ul>
                            <li><a href="#">浙江大学召开学院(系) 工作交流会</a></li>
                            <li><a href="#">浙大师生集中收看江泽民同志追悼大会，深切悼...</a></li>
                            <li><a href="#">校党委书记任少波领办教代会提案见面会举行</a></li>
                            <li><a href="#">发展中国家科学院第16届学术大会暨第30届院士...</a></li>
                            <li><a href="#">建筑设计院荣膺6项世奥建筑新闻网大奖!</a></li>
                            <li><a href="#">基础医学院陈宝惠/潘冬立课题组《Journal of...</a></li>
                            <li><a href="#">基础医学院毛旭明/赵青威课题组合作发文揭示...</a></li>
                            <li><a href="#">其础医学院柯越海/曹倩/肖鹏课题组 《Cellular...</a></li>
                            <h4><a href="#">更多>></a></h4>
                        </ul>
                    </div>
                    <div class="hot_bottom_i1"></div>
                </div>
                <div class="column">
                    <ul>
                        <li><a href="#">图书馆</a></li>
                        <li><a href="#">校友总会</a></li>
                        <li><a href="#">学术进展</a></li>
                        <li><a href="#">书记信箱</a></li>
                        <li><a href="#">电子地图</a></li>
                        <li><a href="#">公开课</a></li>
                        <li><a href="#">教育基金会</a></li>
                        <li><a href="#">创新2030计划</a></li>
                        <li><a href="#">校长信箱</a></li>
                        <li><a href="#">电子邮箱</a></li>
                    </ul>
                </div>
            </div>
            <div class="news_footer">
                <div class="news_footer_left">
                    <div>
                        <p>浙江省杭州市西湖区余杭塘路866号 | 310058 | 0571-87951111 | <a href="#">联系方式</a></p>
                        <p>©2004-2020 浙江大学 <a href="#">浙ICP备05074421号-1 浙公网安备33010602010295</a> | 宣传部维护</p>
                    </div>
                    <ul>
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                    </ul>
                </div>
                <div class="news_footer_right"><a href="#">网站地图</a></div>
            </div>
        </div>
    </div>
</body>
</html>
